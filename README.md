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

-

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
- [VMDE: Virtual Machines Detection Enhanced](https://www.heise.de/downloads/18/1/1/8/3/5/5/9/vmde.pdf)
- [Virtualization Security: Virtual Machine Monitoring and Introspection](https://cdn.ttgtmedia.com/rms/pdf/RHUL_Tsifountidis_Final.pdf) (2011)
- [Malware Virtualization-Resistant Behavior Detection](https://ieeexplore.ieee.org/document/6121379) (December 2011)
- [On the Impossibility of Detecting Virtual Machine Monitors](https://link.springer.com/content/pdf/10.1007/978-3-642-01244-0_13.pdf) (2009)
- [Detecting the Presence of Virtual Machines Using the Local Data Table](https://www.ccoderun.ca/programming/2009-12-30_Virtualization/www.offensivecomputing.net_vm.pdf) (2009)
- [Stealth sandbox analysis of malware](https://repository.bilkent.edu.tr/server/api/core/bitstreams/b40cd415-b27e-4f79-acfd-f8b06d99d439/content) (August 2009)
- [Detecting System Emulators](https://link.springer.com/chapter/10.1007/978-3-540-75496-1_1) (October 2007)
- [On the Cutting Edge: Thwarting Virtual Machine Detection](https://handlers.sans.org/tliston/ThwartingVMDetection_Liston_Skoudis.pdf) (2006)
- [Methods for Virtual Machine Detection](http://charette.no-ip.com:81/programming/2009-12-30_Virtualization/www.s21sec.com_vmware-eng.pdf) (June 2006)

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

### Media

- [LISA15 - Hyperprobe: Towards Virtual Machine Extrospection](https://www.youtube.com/watch?v=dmSQ1R5WCJs)

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

-

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.
