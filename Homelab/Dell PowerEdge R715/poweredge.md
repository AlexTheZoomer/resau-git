---
title: How I Ended up with my Dell PowerEdge R715...
draft: false
tags:
  - Homelab🖥️
---
## Homelab Articles 🌐

[[imessage|Setting up a IMessage Relay Server on a pair of AMD Opteron 6380's - Proxmox]]




---
- [[poweredge#Introduction|Introduction]]
- [[poweredge#Server Software|Server Software]]
	- [[poweredge#<u>Virtual Enviroments</u>|Virtual Enviroments]]
		- [[poweredge#Proxmox VE|Proxmox VE]]
		- [[poweredge#XCP-NG|XCP-NG]]
		- [[poweredge#VMware ESXi|ESXi]]
---

## Introduction

Four years ago now (2020), I came into possession of my now… mostly loved main server `cabot-hugerobot1`, known by most as the Dell PowerEdge R715. This is a Piledriver based 11th generation Dell PowerEdge Server, originally released in 2011 as an AMD K10 Virtualisation host, and database server. 

As currently spec'd, this server includes:

- **2x AMD Opteron 6380 CPU** - 16 Core, 115W 
- **DELL DXTP3 SR5670** Motherboard
- **AMD RX 460 GPU** (*mainly used for MacOS video acceleration*)
- **Matrox G200** Video Accelerator
- **64GB Micron DDR3 1600MHz** Ram 
- **DELL PERC H700 RAID Accelerator**
- **2x 15K SAS DELL Drives - 960GB** (*RAID 1*)
- **2x Micron 5300 Pro - 1TB** (*RAID 0*)
- **4x 1GBPS Broadcom Uplink** (in NIC team)
- **2x DELL G24H2 750W** Power Supply


![[Snapchat-1969669407.jpg|400]]

It's certainly not a new beast, but it's been able to keep up with my lifestyle, and needs. It's been a test bed for my other projects and work, development bed, file and media server, and virtualization host for my local services. Likewise, it lives in the basement, and is hooked up to a generic APC UPS. One day, I hope to install solar to offset the power draw of this box, which can *IDLE* at upwards of 150 Watts. [Could give a 14th Gen Core chip a run for its money..](https://www.anandtech.com/show/21084/intel-core-i9-14900k-core-i7-14700k-and-core-i5-14600k-review-raptor-lake-refreshed/6)... 

![[Snapchat-1099585114.jpg]]

---

# Server Software

#### <u>Virtual Enviroments</u>

>Over the years, I have tried many differing hypervisor solutions, but have ending up sticking with [Proxmox VE](https://www.proxmox.com/en/proxmox-virtual-environment/overview). I have found it's been most reliable, and the only hypervisor *really worth your time*.

![[Pasted image 20240803225025.png]]

##### Proxmox VE

To put it simply, Proxmox VE has been a treat to use. I've been using it since release six, and it's just been plain flexible. I've deployed servers in production, and have other servers at home running Proxmox, and it has been the most powerful and stable solution that I've found so far. Being based on Debian, with a recent enough kernel and a titan of a community, it has been a rock solid option that has an answer to the majority of problems I've run into. 

Being based on Linux, much of the KVM groundwork has been around for a very long time, and is very easily translatable. Projects such as my [[imessage|MacOS Relay Server]] have gone much smoother than previous attempts solely due to the amount of community support and existing KVM resources. Proxmox has been that for me. I've been a huge fan of Proxmox's [[importanceoffoss|FOSS nature]], and the amount of community contribution.  ^acf846

**Proxmox has robust:**

- KVM Management
- LXC (Local Linux Container) Management
- Clustering Support, for larger scale deployments
	- Which includes **Live Migration**
- File Serving Capabilities 
	- (and *every type of storage file system imaginable*)
- Administration Management
	- Integrated **Linux PAM support**
	- Microsoft Active Directory
	- LDAP
	- and an integrated Proxmox Authentication Server (If you want to keep things simple...)
- High Availability Failover (*With HA Failover Simulation!!*)
- Networking (simple VLANs and bonding to *wayyyyyy more complicated stacks*)
- Backup Management 

*And did I mention that this is all free??*

>[!check] The Good 
>- Bonus points for a super robust web UI and mobile app. ➕

 >[!warning] The Eh...
 >- I've had some weird occasional system lockups. I'm *pretty sure* it's the fault of my 13 year old SATA/SAS backplane  🟰

>[!fail] The Bad
>- Disk Migration in between VM's isn't automated, and has proven to be a slight pain in Proxmox. ➖
>- ZFS is slightly weird ➖
>- I'd say a basic knowledge of Linux is required. Things sometimes break.  ➖

---
##### XCP-NG

![[xolist.png]]

Ah… XCP-NG. This is certainly a peculiar one. I ran XCP-NG from March 2021 to December 2022 on `cabot-hugerobot1`, and honestly… I liked it! 

XCP-NG arises from the death of Citrix XenServer, and is based on the [Xen virtual machine framework](https://en.wikipedia.org/wiki/Xen).  Just like [[poweredge#Proxmox VE|Proxmox VE]] currently does for me, XCP-NG ran my main server stack running all of my home and web services for that period of time, with little to no issues. 

![[xenconsole.png]]

Now, XCP certainly has its oddities. XCP-NG comes as a base server, but by default ***has no built-in web UI***. The XCP-NG project runs alongside the [Xen Orchestra](https://xen-orchestra.com/#!/xo-home) (XO) project. The teams seem to share development time and resources, but are two separate entities. XO and XCP-NG are both [[importanceoffoss|FOSS]] pieces of software, so a win in my books, and both have a young, but very passionate community. They were both initially developed as alternatives, and eventually a continuation of XenServer, and you can still see bits of XenServer here and there. 

![[f9a2c7a4-e1dd-44d5-876f-ae9e6fb9f7f4-grafik.png]]

XCP-NG Center is an example of this. It is a piece of depreciated software in the eyes of the main developers, but still has quite a bit of community attention on it. While XO is a “ground-up” new web UI for the XCP-NG platform, XCP-NG Center is fork of the old XenCenter manager for XenServer. Visually and functionally, they are very similar. This was a piece of software that I used quite a bit when I first got into XCP, as XO wasn't as mature at the time. 

**XCP-NG has robust:**

- Xen VM Management
- Clustering Support, for larger scale deployments
	- Which includes **Live Migration**
- File Serving Capabilities 
	- (and *every type of storage file system imaginable*)
- VM Migration Support (from other virtualisation solutions, however not really live…)
- High Availability Failover (kind of…)
- Networking (Slightly simpler than Proxmox)
- Backup Management

Overall, XCP-NG is slightly more basic than Proxmox, while being a tad bit more “new user” friendly.  

>[!check] The Good
>- I loved the ease of use, and stability. Funnily enough, XCP-NG crashed the least out of all of the solutions listed. I had maybe a day or two of downtime over the year. ➕

 >[!warning] The Eh...
 >- While being easy to use, I found XO to be a bit too... simple. Lacking some features at the time compared to XCP-NG Center.  🟰
 >- My [[imessage|MacOS Relay Server]] never stood a chance of working on here. There have been no efforts getting MacOS to boot on Xen. 🟰
 >- Performance was... weird on some instances to say. I don't quite know what to chalk this up to, but Ram and Disk IO was frequently lower than expected. 🟰
 
>[!fail] The Bad
>- Windows Virtual Machines are basically a write-off. Messing with Secure Boot, UEFI and the client Xen Tools was bad enough, and Windows 11 is a **ROYAL** pain with the TPM requirements. ➖
>- iSCSI was a massive pain. ➖
>- Migration and failover isn't really "live", it's more of  a  "warm migration". The idea is you migrate things over, shut down the VM briefly, and then move the last bit of data over and start it up on XCP. ➖

---
##### VMware ESXi

![[VMwareESXiHostClientSummary.png]]

To begin, I have very mixed feelings about ESXi. 

ESXi used to be ***great*** and there was a reason why everybody used to use it. It truly was the best solution at the time, and could do anything any business, large to small, would ever need. I deployed ESXi 6.3, and eventually 7.0 briefly on `cabot-hugerobot1` from January 2020 to Febuary 2021, a couple of years before everything went to *crap* ([cough, cough](https://www.computerworld.com/article/1612211/killing-vmware.html)). Truthfully, VMware was heading in the Adobe direction of laying down the subscription model long before Broadcom showed up, but they certainly did not make it any better. 

Free availability of ESXi died on [Jul 9, 2024](https://knowledge.broadcom.com/external/article/345098/end-of-general-availability-of-the-free.html) making so mandatory to purchase a license in order to use anything VSphere. (*yet, they made [Workstation Pro free](https://blogs.vmware.com/workstation/2024/05/vmware-workstation-pro-now-available-free-for-personal-use.html)?? Truly an odd company…*) Those who held free licenses before the cutoff, to my understanding, got grandfathered in. I'm pretty sure I'm in that camp, not that I'd care to look.

ESXi is not [[importanceoffoss|FOSS]], but did use to be free. It was a great entryway into the VMware portfolio for hobbyists, so I really do not understand why they killed that.   

EXSi is not based on Linux like the other two solutions, but is based on a custom tailored version of BSD developed in house by VMware. Being based on a custom UNIX, it was quite a stable solution, but with tigher hardware support than the other two. I imagine this was also in place due to agreements with vendors such Dell, HP, and Cisco.  Officially, `cabot-hugerobot1` lost support at 6.3, but I was able to boot up to 7.2, with those backplane crashes showing up once I did so. 

![[VMware-vCenter-Server-with-a-vSphere-cluster.png]]

ESXi was very tightly-knit with VMware's other [VSphere](https://en.wikipedia.org/wiki/VMware_vSphere) offerings with VCenter being what I used most. Everything is controlled by licensing, so you are only getting what you pay for. ESXi was quite pain free to use, both in the web UI, and in VCenter.

We have gone our separate ways, but ESXi *used* to be a cool kid on the block. No longer. 

>[!check] The Good
>- Very easy to use, stable, and integrated piece of software. I could see how a large hyperscaler, or large business would find this attractive.  ➕

 >[!warning] The Eh...
 >- No free option at all anymore, post 2024. 🟰

>[!fail] The Bad
>- Broadcom, and by extension VMware, no longer cares about its hobbyist crowd that uses ESXi at home. They have proven to be active aggressors against those who are trying to do so. ➖
>- Homegrown community has fallen apart, and moved elsewhere. There have been no really active forums since early summer of 2024. ➖
>- ESXi, and by extension, VSphere in its entirety, doesn't give you very much flexibility, or room to tinker. Especially with the custom UNIX base, it's a very locked down system.  ➖
>- And finally, they are constantly depreciating old hardware (not even that old! 5ish year old systems are being dumped off the support list). Not acceptable for enterprise hardware. ➖ 


---