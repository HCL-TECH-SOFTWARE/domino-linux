---
layout: default
title: "Will not work"
nav_order: 3
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

There are several AHA ideas out there - please vote for them if you want HCL Domino to be supporting ARM CPU's 
* [ARM version of Domino Server on Linux ](https://domino-ideas.hcltechsw.com/ideas/DOMINO-I-2285)
* [Domino on Docker in the ARM based Apple M1/M2/M3](https://domino-ideas.hcltechsw.com/ideas/DOMINO-I-2387) 
* [Domino Designer for ARM](https://domino-ideas.hcltechsw.com/ideas/NTS-I-1897)

### How about Emulators?
We have tested running the x86 version of Domino on ARM CPU's in compatibility mode. While it is somewhat possible, e.g. in a docker container, it is not fun to work with as performance is 10x slower.