---
layout: default
title: "Will not work"
nav_order: 4
description: "What will not work"
has_children: false
---

<h1>What will not work</h1>
Lessons learned on what will NOT work.

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## ARM CPU
HCL Domino is not compiled for ARM CPU's and will not work on the following hardware
* Raspberry Pi
* Intel Atom CPU's
* Amazon EC2 Graviton
* Apple Silicon (M1/M2/M3/M4 CPU's)

There are several AHA ideas out there - please vote for them if you want HCL Domino to be supporting ARM CPU's 
* [ARM version of Domino Server on Linux ](https://domino-ideas.hcltechsw.com/ideas/DOMINO-I-2285)
* [Domino on Docker in the ARM based Apple Silicon M1/M2/M3/M4](https://domino-ideas.hcltechsw.com/ideas/DOMINO-I-2387) 
* [Domino Designer for ARM](https://domino-ideas.hcltechsw.com/ideas/NTS-I-1897)

### How about Emulators?
We have tested running the x86 version of Domino on ARM CPU's in compatibility mode. While it is somewhat possible, e.g. in a docker container, it is not fun to work with as performance is 10x slower.

## Mainframe / zLinux / zOS
HCL Domino is not compiled for Mainframe CPUs and will NOT work on the following 
* OS/390 - although older versions of Domino used to support z/OS, see this [IBM Redbook](https://www.redbooks.ibm.com/abstracts/sg245984.html)
* IBM zLinux
* IBM LinuxOne
* [IBM Telum](https://en.wikipedia.org/wiki/IBM_Telum)

Please vote this idea if you want HCL Domino to be supporting Mainframes
* [Support for Domino on z/OS / zLinux ](https://domino-ideas.hcltechsw.com/ideas/DOMINO-I-325)
