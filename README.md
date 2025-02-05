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

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

### Media

-

<p align="center"><a href="#contents"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>

## :wrench: Tools

Tools are divided into their respective categories (by default, all tools are in user-mode):

- 🐧: Linux
- 🪟: Windows
- 🍏: macOS
- 💽: raw / no OS / UEFI
- 🚀: kernel-mode

Start of the list:

- 🐧🪟🍏 | [VMAware](https://github.com/kernelwernel/VMAware) : Easy-to-use cross-platform C++ VM detection library and tool
- 🪟 | [Pafish](https://github.com/a0rtega/pafish) : testing tool that uses different techniques to detect virtual machines and malware analysis environments in the same way that malware families do.
- 🪟 | [VMDE](https://github.com/hfiref0x/VMDE) : Virtual Machines Detection Enhanced, source from VMDE paper, adapted to 2015. See [original paper](https://github.com/hfiref0x/VMDE/blob/master/bin/vmde.pdf).
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

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.
