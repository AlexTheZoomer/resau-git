---
title: Project Archive  —  Alexandre DesAulniers
draft:
tags:
  - Introductions
aliases:
---

<p style="padding-bottom:10px;"></p>

<center><h2>Project Archive  —  Alexandre DesAulniers</h2></center>
&nbsp;


![[cover1.png|center|270]]
<p style="padding-top:20px;"></p>

Welcome to my Project Archive! This space documents my some displays some of my work through various technical and creative disciplines, highlighting both completed works and ongoing endeavors. 

Feel free to explore my documentation describing how I bring ideas to life!

[GitHub](https://github.com/a-desaulniers) | [[Papers/] |Papers/]]
## Quick Guide 

- [[projects#"HMCS Sackville" Self Pathing ROS2 Droid 🤖|HMCS Sackville" Self Pathing ROS2 Droid 🤖]]
- [[projects#DSB-SC - AM, FSK Transmitter 📻|DSB-SC - AM, FSK Transmitter 📻]]
- [[projects#AMD BC250 Nodes - Accelerated HCP Cluster 💽|AMD BC250 Nodes - Accelerated HCP Cluster 💽]]
- [[projects#Dell PowerEdge R715 - `hugeRobot` Virtualization Host 🌐|Dell PowerEdge R715 - hugeRobot Virtualization Host 🌐]]
- [[projects#Dalhousie FSAE - CFD Compute 🏎️|Dalhousie FSAE - CFD Compute 🏎️]]
- [[projects#Buck Boost, Transient Voltage Regulation Power Supply Design 🔋⚡|Buck Boost, Transient Voltage Regulation Power Supply Design 🔋⚡]]
- [[projects|Quebec Innovative - White Hydrogen, Early Investor 🫧]]
---
## `sackville`Self Pathing ROS2 Droid 

![[Pasted image 20260217220053.png|400]]![[Pasted image 20260217221616.png|215]]

[sackville - GitHub](https://github.com/a-desaulniers/ECED3901_sackville)

`sackville` is a very neat little project of ours, yet to be completed in tandem with good friends Michael Doyle, Andrew Franklin, Owen Melanson, and Assadah Kausar. At its core, `sackville` is primarily a path-finding robot that utilizes LiDAR triangulation, ultrasonic sounding, and ROS2 instructions to determine its position in space and navigate courses. Designed as a delivery robot, `sackville` aims to path-find to a container, pick it up, navigate back, and drop it off in a predetermined region.

To date, I have contributed to the auxiliary power systems design, UART sensor datastreaming, and Linux workflow management. These contributions are detailed below:

>[!tip] NiMH 2.4V Boost, Transient Voltage Regulation Power Supply Design
>Designed to power all core subsystems, `sackville` required a ***very*** steady 5V rail, as it was entirely responsible for powering sensitive sensor equipment on board. Panasonic NiMH 2000mAh cells were chosen to power these systems due to the nature of `sackville`'s testing and evaluation process, where dead battery cells during testing and presentation were not an option. I designed a system around a 500kHz switching IC - the Texas Instruments TPS61288, which was chosen for its flexible input voltage and accompanying low dropout voltage.
>
>
>![[Circuit Diagram.png|center|400]]
> <center><sup><sub>Circuit Schematic, based on Texas Instruments TPS61288</sub></sup></center>
>
>As previously mentioned, stable 5V output with as little ripple as possible was required for the robot's imaging, LiDAR, and ultrasonic systems, which are hugely susceptible to noise.
>
>Given that the TPS61288 is a switching boost, achieving this was difficult. Through FFT Analysis and LTSpice unit tests, a design was implemented operating at a mean 98.24% efficiency across the operational range (0–1.667A). This configuration safely provides up to 2.35A at a steady 5V from the cells, tested with a decaying transient 2.8V–2.0V input.


![[chart.png|350]]![[chart(2).png|350]]
<center><sup><sub>Recorded Ripple & Transfer Efficiency Characteristics</sub></sup></center>


![[Pasted image 20260217211531.png|center|400]]
<center><sup><sub>FFT Output Analysis</sub></sup></center>

![[Pasted image 20260217211806.png|center|600]]
<center><sup><sub>Steady State Vout Load Ripple, Across Increasing Load Conditions </sub></sup></center>

![[Pasted image 20260217212042.png|center|600]]
<center><sup><sub>Steady State Vout Load Ripple  </sub></sup></center>

>[!example] UART Sensor Data Pipeline
>
>With the navstack team requiring huge swaths of location data to assist in conditionality compute, I implemented the primary 14.4 KB/s UART data streams connecting the primary compute board and multiple ATMega328P data stream input MCUs. In the process, I wrote a serial bridge driver for ROS2, publishing MCU sensor data onto a ROS publisher topic to be accessed by the navstack team. This driver is able to handle up to 400 location polls a second.
>
>The driver itself is a custom C++ ROS2 node that interfaces directly with the Linux serial device, targeting `/dev/ttyUSBX`. The implementation uses a 10ms timer loop to poll the serial port, reading raw buffer data and converting it into `std_msgs::msg::Int32` format. I included a basic try-catch block within the `read_serial` function to catch any UART garbled partial lines that might result from timing desyncs, ensuring the final published ROS topic only receives clean data. 
>
>The bridge links `sackville`'s MCU hardware sensors directly into  ROS2, providing the high-frequency distance polling for real-time obstacle avoidance during navigation.

---
## Homemade FSK AM Transmitter 

![[Pasted image 20260217225901.png|center|500]]

This project involved developing a custom communication link to transmit digital data using Frequency Shift Keying. It’s a custom-built.. prehistoric modem that allows an ATMega328P to broadcast bit-streams by toggling between distinct frequencies to represent logic '1' and '0'. The hardware, assembled on the compact perfboard as shown below, eventually put on a PCB, was designed to provide a semi-reliable data link over an analog medium. 

The transmitter uses a custom direct digital synthesis engine written in AVR C to produce a clean signal. Due to the lack of a proper preexisting sine function in AVR C on lower end Atmel hardware, I implemented a 64-point sine wave lookup table scaled for 8-bit PWM. This is handled by the Atmel's Timer0 in Fast PWM mode, outputting the synthesized wave as a varying duty cycle square wave, smoothed out with an RC Circuit to produce the desired wave. 

To prevent drifting in the transmission timing, I implemented a dual-interrupt architecture:

- **Signal Generation:** The overflow interrupt handles the high-frequency task of cycling the sine table, mapped to Timer0. Frequency is adjusted on the fly by scaling the `OCR0A` value; a logical '1' is mapped to **57Hz**, while a logical '0' is mapped to **107Hz**. 
    
- **Bit Timing:** This timer acts as the bit-clock, carried out by Timer1. Every 20,000 cycles, the ISR pulls the next bit from the message array and updates the carrier frequency accordingly.
    
This was certainly an early low frequency endeavor on a homemade transmitter coil (*iron core and hand twisted copper wire)*, but a 10m transmission could happily be read via an adjacent ADC. A bit more time, and knowledge with analog filter design would have gotten me a lot farther. This was a second year project, after all. 

![[Pasted image 20260217230033.png]]
<center><sup><sub>Each Jump appears very distinct at 107hz </sub></sup></center>

---
## AMD BC250 Nodes - Accelerated HCP Cluster


## Dell PowerEdge R715 - `hugeRobot` Virtualization Host

![🗃️ Dell PowerEdge R715 Restoration | Homelab Project](poweredge.md)


## Dalhousie FSAE - CFD Compute Node 

Dell PowerEdge R740, Nvidia RTX A4000

![[Pasted image 20260217210228.png|300![[Pasted image 20260217211105.png]]





