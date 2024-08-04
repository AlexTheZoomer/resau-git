---
title: How I Ended up with my Dell PowerEdge R715...
draft: false
tags:
  - Homelab🖥️
---
# Table Of Contents

- [[poweredge#Introduction|Introduction]]
- [[poweredge#Server Software|Server Software]]

---

### Introduction

Four years ago now (2020), I came into possession of my now... mostly loved main server `HugeRobot`, known by most as the Dell PowerEdge R715. This is a Piledriver based 11th generation Dell PowerEdge Server, originally released in 2011 as an AMD K10 Virtualisation host, and database server. 

As currently spec'd, this server includes:

- **2x AMD Opteron 6380 CPU** - 16 Core, 115W 
- **DELL DXTP3 SR5670** Motherboard
- **AMD RX 560 GPU** (*mainly used for MacOS video acceleration*)
- **Matrox G200** Video Accelerator
- **64GB Micron DDR3 1600MHz** Ram 
- **DELL PERC H700 RAID Accelerator**
- **2x 15K SAS DELL Drives - 960GB** (*RAID 1*)
- **2x Micron 5300 Pro - 1TB** (*RAID 0*)
- **4x 1GBPS Broadcom Uplink** (in NIC team)
- **2x DELL G24H2 750W** Power Supply


![[Snapchat-1969669407.jpg|400]]

It's certainly not a new beast, but it's been able to keep up with my lifestyle, and needs. It's been a test bed for my other projects and work, development bed, file and media server, and virtualisation host for my local services. Likewise, it lives in the basement, and is hooked up to a generic APC UPS. One day, I hope to install solar to offset the power draw of this box, which can *IDLE* at upwards of 150 Watts. [Could give a 14th Gen Core chip a run for its money..](https://www.anandtech.com/show/21084/intel-core-i9-14900k-core-i7-14700k-and-core-i5-14600k-review-raptor-lake-refreshed/6)... 

![[Snapchat-1099585114.jpg]]

---

### Server Software

Over the years, I have tried many differing hypervisor solutions, but have ending up sticking with [Proxmox VE](https://www.proxmox.com/en/proxmox-virtual-environment/overview). I have found it's been most reliable, and the only hypervisor *really worth your time*.

![[Pasted image 20240803225025.png]]

##### Proxmox VE

To put it simply, Proxmox VE has been a treat to use. I've been using it since release six, and it's just been plain flexible. I've deployed servers in production, and have other servers at home running Proxmox, and it has been the most powerful and stable solution that I've found so far. Being based on Debian, with a recent enough kernel and a titan of a community, it has been a rock solid option that has an answer to the majority of problems I've run into. 

Being based on Linux, much of the KVM groundwork has been around for a very long time, and is very easily translatable. Projects such as my [[imessage|MacOS Relay Server]] have gone much smoother than previous attempts solely due to the amount of community support and existing KVM resources. Proxmox has been that for me. Proxmox's FOSS nature has been 