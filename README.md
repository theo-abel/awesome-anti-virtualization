# Awesome Anti-Virtualization [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) <a href="https://x.com/intent/post?text=Awesome Anti Virtualization - A curated list of awesome resources related to anti virtualization techniques.%0D%0Ahttps://github.com/standard3/awesome-anti-virtualization%0D%0A&hashtags=awesomelists%2Cantivm%2Cantivmdetection%2Cantivirtualization%2Ccybersecurity%2Cinfosec"><img src="https://img.shields.io/badge/Tweet--lightgrey?logo=x&style=social" alt="Tweet" height="20"/></a>

> A curated list of resources related to anti-virtualization techniques containing references to books, papers, blog posts, and other written resources.

Anti-virtualization techniques are used to detect and evade virtualized environments. These techniques are used by malware authors, anti-cheats and proprietary software among others to avoid detection by security researchers and analysts.

We generally divide anti-virtualization techniques (also called anti-VM or redpills) into 4 categories:

- **Timing-based**: These techniques rely on the fact that virtualized environments have different timing characteristics than physical machines.
- **Behavior-based**: These techniques rely on the fact that virtualized environments have different behaviors than physical machines.
- **Signature-based**: These techniques rely on the fact that virtualized environments have different signatures than physical machines.
- **Based on a trusted third party**: These techniques rely on the fact that virtualized environments have a trusted third party that can be used to detect them.

These techniques can be called redpills because they are used to detect the "red pill" of a virtualized environment. The term "red pill" comes from the movie "The Matrix" where the red pill is used to wake up the protagonist from the virtual world.

> The red pill is a special case of the related "trusted computing" and the attestation concept (Zaidenberg et al. 2015d), In Trusted computing attestation a remote 3rd party or even local software tries to ensure the integrity of the local machine in terms of software (mainly) and hardware (sometimes).
>
> - [Creating Modern Blue Pills and Red Pills, July 2019](https://www.researchgate.net/publication/334988761_Creating_Modern_Blue_Pills_and_Red_Pills)

## Contents

- [:books: Literature](#books-literature) : everything written about anti-virtualization techniques
  - [Documentation](#documentation) (blogs, manuals, specifications, etc.)
  - [Scientific Research](#scientific-research)
  - [Media](#media) (videos, podcasts, etc.)
- [:wrench: Tools](#wrench-tools) : tools to detect and evade virtualized environments
- [:jigsaw: Techniques](#jigsaw-techniques) : a list of anti-virtualization techniques

## :books: Literature

### Documentation

- [About evasion techniques - Check Point Research](https://evasions.checkpoint.com/about/) : A collection of evasion techniques used by malware to avoid detection.
- [Detecting Hypervisor-assisted Hooking - Maurice Heumann](https://momo5502.com/posts/2022-05-02-detecting-hypervisor-assisted-hooking/), see also [Github Project EPT Hook Detection](https://github.com/momo5502/ept-hook-detection/tree/main)
- [Evading ACPI checks in commercial virtualization platforms - Nick Peterson](https://revers.engineering/evading-trivial-acpi-checks/)
- [How anti-cheats detect system emulation - secret.club](https://secret.club/2020/04/13/how-anti-cheats-detect-system-emulation.html)
- [Detecting Hypervisor Presence on Windows 10 - Nick Peterson](https://revers.engineering/detecting-hypervisor-presence-on-windows-10/)
- [7 Ways to Detect Virtualization from your VM \[Xen,VirtualBox,KVM,OpenStack with KVM\] - techglimpse.com](https://techglimpse.com/xen-kvm-virtualbox-vm-detection-command/)
- [Playing with GuLoader Anti-VM techniques - outpost24.com](https://outpost24.com/blog/playing-with-guloader-anti-vm-techniques-malware/)
- [Detecting VMware by reading an invalid MSR - drew](https://howtohypervise.blogspot.com/2018/09/detecting-vmware-by-reading-invalid-msr.html)
- [Defeating malware's Anti-VM techniques (CPUID-Based Instructions) - Sina Karvandi](https://rayanfam.com/topics/defeating-malware-anti-vm-techniques-cpuid-based-instructions/)
- [Deploy Hidden Virtual Machine For VMProtections Evasion And Dynamic Analysis - r0ttenbeef](https://r0ttenbeef.github.io/Deploy-Hidden-Virtual-Machine-For-VMProtections-Evasion-And-Dynamic-Analysis/)

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

### Scientific Research

The following papers are sorted by publication date (newest first):

- [Detection of Virtual Machines Based on Thread Scheduling](https://github.com/kernelwernel/VMAware/blob/d7fa59e1fa7e7a155c24c374a73a51889562e840/papers/Detection%20of%20Virtual%20Machines%20Based%20on%20Thread%20Scheduling.pdf) (July 2021)
- [Hypervisor-assisted dynamic malware analysis](https://cybersecurity.springeropen.com/articles/10.1186/s42400-021-00083-9#Sec11) (June 2021)
- [Resurrecting anti-virtualization and anti-debugging: Unhooking your hooks](http://eprints.bournemouth.ac.uk/34823/1/Anti_forensics.pdf) (March 2021)
- [DBI, debuggers, VM: gotta catch them all: How to escape or fool debuggers with internal architecture CPU flaws?](https://www.researchgate.net/publication/349062549_DBI_debuggers_VM_gotta_catch_them_all_How_to_escape_or_fool_debuggers_with_internal_architecture_CPU_flaws) (June 2021)
- [Creating Modern Blue Pills and Red Pills](https://www.researchgate.net/publication/334988761_Creating_Modern_Blue_Pills_and_Red_Pills) (July 2019)
- [Rethinking anti-emulation techniques for large-scale software deployment](https://daehee87.github.io/data/qemu.pdf) (June 2019)
- [New attack technique based on Meltdown. Using speculative instructions to detect virtualization](https://sudonull.com/post/58475-New-attack-technique-based-on-Meltdown-Using-speculative-instructions-for-detecting-virtualization-B) (May 2018)
- [A Study of I/O Performance of Virtual Machines](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8429117) (June 2017)
- [Detecting Hardware -Assisted Virtualization](https://christian-rossow.de/publications/detectvt-dimva2016.pdf) (July 2016)
- [Virtual Machines Detection Methods Using IP Timestamps Pattern Characteristic](https://www.researchgate.net/publication/297726086_Virtual_Machines_Detection_Methods_Using_IP_Timestamps_Pattern_Characteristic) (February 2016)
- [Two challenges of stealthy hypervisors detection : time cheating and data fluctuations](https://arxiv.org/pdf/1506.04131) (2015)
- [New Methods for Detecting Malware Infections and New Attacks against Hardware Virtualization](https://repozitorium.omikk.bme.hu/items/4c76e047-9d2e-4196-a6c5-e7837c350bc6) (2015)
- [Hyperprobe: Towards Virtual Machine Extrospection](https://www.usenix.org/system/files/conference/lisa15/lisa15-paper-xiao.pdf) (2015), see also [Presentation Video](https://www.usenix.org/conference/lisa15/conference-program/presentation/xiao)
- [An assessment of virtual machine assails](https://www.ijates.com/images/short_pdf/1421766783_P315-320.pdf) (January 2015)
- [Cardinal Pill Testing of System Virtual Machines](https://www.usenix.org/conference/usenixsecurity14/technical-sessions/presentation/shi) (August 2014)
- [An analysis of hardware-assisted virtual machine based rootkits](https://calhoun.nps.edu/server/api/core/bitstreams/9b32dd11-5ad8-4e1b-b085-f7fe27b13fc7/content) (June 2014)
- [VMDE: Virtual Machines Detection Enhanced](https://www.heise.de/downloads/18/1/1/8/3/5/5/9/vmde.pdf) (November 2013)
- [Anti-virtual machines and emulations](http://staff.ustc.edu.cn/~bjhua/courses/security/2014/readings/anti-vm2.pdf) (June 2012)
- [Virtualization Security: Virtual Machine Monitoring and Introspection](https://cdn.ttgtmedia.com/rms/pdf/RHUL_Tsifountidis_Final.pdf) (2011)
- [Malware Virtualization-Resistant Behavior Detection](https://ieeexplore.ieee.org/document/6121379) (December 2011)
- [On the Impossibility of Detecting Virtual Machine Monitors](https://link.springer.com/content/pdf/10.1007/978-3-642-01244-0_13.pdf) (2009)
- [Detecting the Presence of Virtual Machines Using the Local Data Table](https://www.ccoderun.ca/programming/2009-12-30_Virtualization/www.offensivecomputing.net_vm.pdf) (2009)
- [Stealth sandbox analysis of malware](https://repository.bilkent.edu.tr/server/api/core/bitstreams/b40cd415-b27e-4f79-acfd-f8b06d99d439/content) (August 2009)
- [Attacks on More Virtual Machine Emulators](https://pferrie.tripod.com/papers/attacks2.pdf) (2007), see [associated slides](http://pferrie.epizy.com/papers/attacks2.ppt)
- [Attacks on Virtual Machine Emulators](https://www.cityu.edu.hk/its/sites/g/files/asqsls6511/files/media/inline-image/Virtual_Machine_Threats.pdf) (2007), see [associated slides](http://pferrie.epizy.com/papers/attacks.ppt)
- [Detecting System Emulators](https://link.springer.com/chapter/10.1007/978-3-540-75496-1_1) (October 2007)
- [On the Cutting Edge: Thwarting Virtual Machine Detection](https://handlers.sans.org/tliston/ThwartingVMDetection_Liston_Skoudis.pdf) (2006)
- [Methods for Virtual Machine Detection](http://charette.no-ip.com:81/programming/2009-12-30_Virtualization/www.s21sec.com_vmware-eng.pdf) (June 2006)

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

### Media

- [LISA15 - Hyperprobe: Towards Virtual Machine Extrospection](https://www.youtube.com/watch?v=dmSQ1R5WCJs)
- [Don't Tell Joanna, The Virtualized Rootkit Is Dead](https://archive.org/details/2007_BlackHat_Vegas-V18-Ptacek-Ferrie-Lawson-Dont_Tell_Joanna), see [associated slides](http://pferrie.epizy.com/papers/vtrootkits.pdf)

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

## :wrench: Tools

Tools are divided into their respective categories (by default, all tools are in user-mode):

| Icon | Description |
| --- | --- |
| 🐧 | Linux |
| 🪟 | Windows |
| 🍏 | macOS |
| 💽 | raw / no OS / UEFI |
| 🚀 | kernel-mode |

Start of the list:

- 🐧🪟🍏 | [VMAware](https://github.com/kernelwernel/VMAware) : Easy-to-use cross-platform C++ VM detection library and tool
- 🐧 | [Hypervisor-Phantom](https://github.com/Scrut1ny/Hypervisor-Phantom) : Advanced malware analysis tool for evading detection from advanced malware.
- 🪟 | [Pafish](https://github.com/a0rtega/pafish) : testing tool that uses different techniques to detect virtual machines and malware analysis environments in the same way that malware families do.
- 🪟 | [VMDE](https://github.com/hfiref0x/VMDE) : Virtual Machines Detection Enhanced, source from VMDE paper, adapted to 2015.
- 🪟 | [Hypervision-Detection](https://github.com/void-stack/Hypervisor-Detection) : Detects virtual machines and malware analysis environments
- 🪟 | [Al-khaser](https://github.com/ayoubfaouzi/al-khaser) : al-khaser is a PoC "malware" application with good intentions that aims to stress your anti-malware system. It performs a bunch of common malware tricks with the goal of seeing if you stay under the radar.
- 💽🪟 | [illusion-rs](https://github.com/memN0ps/illusion-rs) : Rusty Hypervisor - Windows UEFI Blue Pill Type-1 Hypervisor in Rust (Codename: Illusion)
  - specifically see [Hypervisor detection](https://github.com/memN0ps/illusion-rs?tab=readme-ov-file#hypervisor-detection) section
- 🚀🪟 | [hyperdetect.cc](https://gist.github.com/drew-gpf/d31840bebbbb1ff1d112a6f46e162c05): C++ code snippet that checks for a “lazy” hypervisor running in kernel-mode
- 🪟 | [antivmdetection](https://github.com/nsmfoo/antivmdetection) : Script to create templates to use with VirtualBox to make vm detection harder
- 🪟 | [InviZzzible](https://github.com/CheckPointSW/InviZzzible) : InviZzzible is a tool for assessment of your virtual environments in an easy and reliable way. It contains the most recent and up to date detection and evasion techniques as well as fixes for them.
- 🪟 | [Anti-VM](https://github.com/Print3M/Anti-VM) : C++ Windows-based implementation of several anti-vm techniques used in malware development.
- 🐧 | [apate](https://github.com/vim951/apate) : Apate performs anti-debugging, anti-VM and anti-sandbox tests, to see if your linux system is able to stay under the radar.
- 🐧 | [inside-vm](https://github.com/PicoJr/inside-vm) : Detect if code is running inside a virtual machine (x86 and x86-64 only).
- 🪟 | [EPT Hook Detection](https://github.com/momo5502/ept-hook-detection)
- 🪟 | [PyDefender](https://github.com/EvilBytecode/PyDefender/tree/main) : Anti Virtulization, Anti Debugging, AntiVM, Anti Virtual Machine, Anti Debug, Anti Sandboxie, Anti Sandbox, VM Detect package for Python.
- 🪟 | [GoDefender](https://github.com/EvilBytecode/GoDefender/) : Anti Virtulization, Anti Debugging, AntiVM, Anti Virtual Machine, Anti Debug, Anti Sandboxie, Anti Sandbox, VM Detect package for Go. Windows ONLY.
- 🐧🪟 | [Metasploit](https://www.metasploit.com/) : Open-source penetration testing framework that includes virtual machine detection modules
  - [metasploit-framework/modules/post/linux/gather/checkvm.rb](https://github.com/rapid7/metasploit-framework/blob/master/modules/post/linux/gather/checkvm.rb)
  - [metasploit-framework/modules/post/windows/gather/checkvm.rb](https://github.com/rapid7/metasploit-framework/blob/master/modules/post/windows/gather/checkvm.rb)
  - [metasploit-framework/scripts/meterpreter/winenum.rb](https://github.com/rapid7/metasploit-framework/blob/master/scripts/meterpreter/winenum.rb#L182)
  - [metasploit-framework/modules/auxiliary/scanner/netbios/nbname.rb](https://github.com/rapid7/metasploit-framework/blob/master/modules/auxiliary/scanner/netbios/nbname.rb#L92)
- 🐧 | [systemd-detect-virt (man page)](https://www.freedesktop.org/software/systemd/man/latest/systemd-detect-virt.html) : `systemd-detect-virt` detects execution in a virtualized environment. It identifies the virtualization technology and can distinguish full machine virtualization from container virtualization. `systemd-detect-virt` exits with a return value of 0 (success) if a virtualization technology is detected, and non-zero (error) otherwise.
  - See also `systemd` code [systemd/src/basic/virt.c](https://github.com/systemd/systemd/blob/main/src/basic/virt.c#L24)

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

## :jigsaw: Techniques
🐧
🪟
🍏

🐧🪟🍏

| Technique | Description | Certainty | Platform | Reference |
| --------- | ----------- | --------- | -------- | --------- |
| VMID | Check CPUID output of manufacturer ID for known VMs/hypervisors at leaf 0 and 0x40000000-0x40000100 | 100% | 🐧🪟🍏 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2525
| CPU brand | Check if CPU brand model contains any VM-specific string snippets | 50% | 🐧🪟🍏 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2545
| Hypervisor bit | Check if hypervisor feature bit in CPUID eax bit 31 is enabled (always false for physical CPUs) | 100% | 🐧🪟🍏 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2601
| Hypervisor string | Check for hypervisor brand string length (would be around 2 characters in a host machine) | 75% | 🐧🪟🍏 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2622
| Timer | Check for timing anomalies in the system | 45% | 🐧🪟🍏 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L8169 
| Thread count | Check if there are only 1 or 2 threads, which is a common pattern in VMs with default settings (nowadays physical CPUs should have at least 4 threads for modern CPUs) | 35% | 🐧🪟🍏 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2649
| MAC address | Check if mac address starts with certain VM designated values | 20% | 🐧🪟 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2671
| Temperature | Check if thermal directory in linux is present, might not be present in VMs | 15% | 🐧 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2804
| Chassis vendor | Check if the chassis vendor is a VM vendor | 65% | 🐧 | https://github.com/kernelwernel/VMAware/blob/8cb2491b1c7d2cb7300d1d698b7c64c953b4ae75/src/vmaware.hpp#L2671
| Chassis type | Check if the chassis type is valid (it's very often invalid in VMs) | 20% | 🐧 | 
| /.dockerenv | Check if /.dockerenv or /.dockerinit file is present | 30% | 🐧 | 
| dmidecode output | Check if dmidecode output matches a VM brand | 55% | 🐧 |  
| dmesg output | Check if dmesg output matches a VM brand | 55% | 🐧 |  
| /sys/class/hwmon | Check if /sys/class/hwmon/ directory is present. If not, likely a VM | 35% | 🐧 | 
| 5th sidt byte | Check if the 5th byte after sidt is null | 45% | 🐧 | 
| DLL | Check for VM-specific DLLs | 25% | 🪟 | 
| Registry |  Check for VM-specific registry values | 50% | 🪟 |
| VM files | Find for VM-specific specific files | 25% | 🪟 |
| hwmodel | Check if the sysctl for the hwmodel does not contain the "Mac" string | 100% | 🍏 |
| Disk size | Check if disk size is under or equal to 50GB | 60% | 🐧 |
| RAM and disk size VBox | Check for default RAM and DISK sizes set by VirtualBox | 25% | 🐧🪟 |
| VBox network | Check for VirtualBox network provider string | 100% | 🪟 |
| Computer name | Check if the computer name (not username to be clear) is VM-specific | 10% | 🪟 |
| Wine file | Check wine_get_unix_file_name file for Wine | 100% | 🪟 |
| Hostname | Check if hostname is specific | 10% | 🪟 |
| KVM directories | Check for KVM directory "Virtio-Win" | 30% | 🪟 |
| QEMU directories | Check for QEMU-specific blacklisted directories | 30% | 🪟 |
| Power capabilities | Check what power states are enabled | 50% | 🪟
| Disk drive ID | Checks for virtual machine signatures in disk drive device identifiers | 100% | 🪟 |
| VM processes | Check for any VM processes that are active | 15% | 🪟 |
| User and hostname | Check for default VM username and hostname for linux | 10% | 🐧 |
| Gamarue | Check for Gamarue ransomware technique which compares VM-specific Window product IDs | 10% | 🪟 |
| Bochs faulty CPU | Check for various Bochs-related emulation oversights through CPU checks | 100% | 🐧🪟🍏 |
| MSSMBIOS | Check MSSMBIOS registry for VM-specific signatures | 100% | 🪟 |
| Low memory | Check if memory is too low for MacOS system | 15% | 🍏 |
| IO kit | Check MacOS' IO kit registry for VM-specific strings | 100% | 🍏 |
| ioreg command | Check for VM-strings in ioreg commands for MacOS | 100% | 🍏 |
| System Integrity Protection | Check if System Integrity Protection is disabled (likely a VM if it is) | 40% | 🍏 |
| HKLM | Check HKLM registries for specific VM strings | 25% | 🪟 |
| QEMU process | Check for "qemu-ga" process | 10% | 🐧 |
| VirtualPC backdoor | Check for official VPC method | 75% | 🪟 |
| sidt instruction | Check for sidt instruction method | 25% | 🪟 |
| sgdt instruction | Check for sgdt instruction method | 30% | 🪟 |
| sldt instruction | Check for sldt instruction method | 15% | 🪟 |
| Offensive Security sidt | Check for Offensive Security SIDT method | 60% | 🪟 |
| Offensive Security sgdt | Check for Offensive Security SGDT method | 60% | 🪟 |
| Offensive Security sldt | Check for Offensive Security SLDT method | 20% | 🪟 |
| VirtualPC sidt | Check for sidt method with VPC's 0xE8XXXXXX range | 15% | 🪟 |
| VMware iomem | Check for VMware string in /proc/iomem | 65% | 🐧 |
| VMware ioports | Check for VMware string in /proc/ioports | 70% | 🐧 |
| VMware scsi | Check for VMware string in /proc/scsi/scsi | 40% | 🐧 |
| VMware dmesg | Check for VMware-specific device name in dmesg output | 65% | 🐧 |
| VMware str instruction | Check str assembly instruction method for VMware | 35% | 🪟 | 
| VMware IO port backdoor | Check for official VMware io port backdoor technique | 100% | 🪟 | 
| VMware memory IO port | Check for VMware memory using IO port backdoor | 85% | 🪟 | 
| smsw instruction| Check for SMSW assembly instruction technique | 30% | 🪟 | 
| Mutex strings | Check for mutex strings of VM brands | 85% | 🪟 |
| Odd CPU threads | Check for odd CPU threads, usually a sign of modification through VM setting because 99% of CPUs have even numbers of threads | 80% | 🐧🪟🍏 |
| Intel thread mismatch | Check for Intel CPU thread count database if it matches the system's thread count | 95% | 🐧🪟🍏 |
| Xeon thread mismatch | Same as above, but for Xeon Intel CPUs | 95% | 🐧🪟🍏 |
| Nettitude VM memory | Check for memory regions to detect VM-specific brands | 100% | 🪟 |
| Cuckoo directory | Check for cuckoo directory using crt and WIN API directory functions | 30% | 🪟 |
| Cuckoo pipe | Check for Cuckoo specific piping mechanism | 30% | 🪟 |
| Hyper-V hostname | Check for default Azure hostname format regex (Azure uses Hyper-V as their base VM brand) | 30% | 🐧🪟 |
| General hostname | Check for commonly set hostnames by certain VM brands | 10% | 🐧🪟 |
| Screen resolution | Check for pre-set screen resolutions commonly found in VMs | 20% | 🪟 |
| Device string | Check if bogus device string would be accepted | 25% | 🪟 |
| BlueStacks folders |  Check for the presence of BlueStacks-specific folders | 5% | 🐧 |
| CPUID signature | Check for signatures in leaf 0x40000001 in CPUID | 95% | 🐧🪟🍏 |
| KVM bitmask | Check for KVM CPUID bitmask range for reserved values | 40% | 🐧🪟🍏 |
| Intel KGT signature | Check for Intel KGT (Trusty branch) hypervisor signature in CPUID | 80% | 🐧🪟🍏 |
| QEMU DMI | Check for presence of QEMU in the /sys/devices/virtual/dmi/id directory | 40% | 🐧 |
| QEMU USB | Check for presence of QEMU in the /sys/kernel/debug/usb/devices directory | 20% | 🐧 |
| Hypervisor directory | Check for presence of any files in /sys/hypervisor directory | 20% | 🐧 |
| User Mode Linux CPU | Check for the "UML" string in the CPU brand | 80% | 🐧 |
| kmsg logs | Check for any indications of hypervisors in the kernel message logs | 5% | 🐧 |
| Xen VM processes | Check for a Xen VM process | 10% | 🐧 |
| VBox kernel module | Check for a VBox kernel module | 15% | 🐧 |
| sysinfo process | Check for potential VM info in /proc/sysinfo | 15% | 🐧 |
| Device tree | Check for specific files in /proc/device-tree directory | 20% | 🐧 |
| DMI scan | Check for string matches of VM brands in the linux DMI | 50% | 🐧 |
| SMBIOS VM bit | Check for the VM bit in the SMBIOS data | 50% | 🐧 |
| Podman file | Check for podman file in /run/ | 5% | 🐧 |
| WSL process | Check for WSL or microsoft indications in /proc/ subdirectories | 30% | 🐧 |
| ANY.RUN driver | Check for any.run driver presence | 65% | 🪟 |
| ANY.RUN directory | Check for any.run directory and handle the status code | 35% | 🪟 |
| Driver names | Check for VM-specific names for drivers | 100% | 🪟 |
| sidt base | Check for unknown IDT base address | 100% | 🪟 |
| HDD serial | Check for serial numbers of virtual disks | 100% | 🪟 |
| Port connections | Check for physical connection ports | 25% | 🪟 |
| GPU capabilities | Check for GPU capabilities related to VMs | 100% | 🪟 |
| GPU VM strings | Check for specific GPU string signatures related to VMs | 100% | 🪟 |
| VM devices | Check for VM-specific devices | 45% | 🪟 |
| idt and GDT scan | Check if the IDT and GDT virtual base addresses are equal across different CPU cores when not running under Hyper-V | 50% | 🪟 |
| Processor count | Check for number of processors | 50% | 🪟 |
| Core count | Check for number of cores | 50% | 🪟 |
| ACPI temperature | Check for device's temperature | 25% | 🪟 |
| Processor ID | Check if any processor has an empty Processor ID using SMBIOS data | 25% | 🪟 |
| QEMU /sys/ | Check for existence of "qemu_fw_cfg" directories within /sys/module and /sys/firmware | 70% | 🐧 |
| lshw QEMU | Check for QEMU string instances with lshw command | 80% | 🐧 |
| Virtual processors | Check if the number of virtual and logical processors are reported correctly by the system | 50% | 🪟 |
| Hyper-V query | Check if a call to NtQuerySystemInformation with the 0x9f leaf fills a _SYSTEM_HYPERVISOR_DETAIL_INFORMATION structure | 100% | 🪟 |
| VM memory pools | Check for system pools allocated by hypervisors | 80% | 🪟 |
| AMD SEV | Check for AMD-SEV MSR running on the system | Linux and MacOS | 50% | 🐧🍏 |
| AMD thread count mismatch | Check for AMD CPU thread count database if it matches the system's thread count | 95% | 🐧🪟🍏 |
| Native VHD | Check for OS being booted from a VHD container | 100% | 🪟 |
| Virtual registry | Check for particular object directory which is present in Sandboxie virtual environment but not in usual host systems | 65% | 🪟 |
| Firmware signatures | Check for VM signatures and patched strings by hardeners in firmware, while ensuring the BIOS serial is valid | 75% | 🪟🐧 |
| File access history | Check if the number of accessed files are too low for a human-managed environment | 15% | 🐧 |
| Audio device | Check if audio device is present | 25% | 🪟 |
| Unrecognised x86 CPU manufacturer | Check if the CPU manufacturer is not known | 50% | 🐧🪟🍏 |
| OSXSAVE | Check if running xgetbv in the XCR0 extended feature register triggers an exception | 50% | 🪟 |
| nsjail PID | Check if process status matches with nsjail patterns with PID anomalies | 75% | 🐧 |
| PCIe bridge name | Check for PCIe bridge names for known VM keywords and brands | 100% | 🐧 |
























<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.
