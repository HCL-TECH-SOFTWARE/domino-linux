---
layout: default
title: "Home"
nav_order: 1
description: "HCL Domino Linux"
has_children: true
---

<h1>Welcome</h1>
This is a documentation-only repository - it describes how to run HCL Domino on the various Linux distributions.

<details close markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Background
The system requirements for HCL Domino include RHEL/CentOS and SUSE because those are the releases that HCL has tested (aka "certified") to run on. However, HCL Domino will run on other distributions if a certain minimum criteria is met. This repository is documenting which flavours of Linux is running on and what customers have to be aware of.

## Compatibility
Overview of which Linux distribution is compatible with which Domino release.

### Dependencies
Overview of HCL Domino dependencies

Domino Version | Kernel Version | min.glibc Version | min stdc++ Version | Remarks
------| :---: | :---: | :---:
HCL Domino 14.0.x | ? | ? | ?
HCL Domino 12.0.x | ? | ? | ?
HCL Domino 11.0.x | ? | ? | ?
HCL Domino 10.0.x | ? | ? | ?
HCL Domino 9.0.x | ? | ? | ?
HCL Domino 8.5.x | ? | ? | ?

### Domino Compatibility
This table provides the collective knowledge of which distribution are known to be working with a Domino version

Distribution | Domino 14 | Domino 12 | Domino 11 
:-------|---|---|---
[SUSE Leap](leap.md) | Incompatible <br /> {: .label .label-red } {: .bg-red-300 } | Works <br /> {: .bg-green-000 } | Works {: .bg-green-000 }
[Redhat Enterprise Linux 9 (RHEL)](rhel.md) | {: .bg-green-000 } | {: .bg-green-000 } | {: .bg-green-000 }
[Redhat Enterprise Linux 8 (RHEL)](rhel.md) | {: .bg-red-300 } | {: .bg-green-000 } | {: .bg-green-000 }
[CentOS Stream 9](centos.md)| {: .bg-green-000 } | {: .bg-green-000 } | {: .bg-green-000 }
[CentOS Stream 8](centos.md)| {: .bg-red-300 } | {: .bg-green-000 } | {: .bg-green-000 }
[CentOS Stream 7](centos.md)| {: .bg-red-300 } | {: .bg-yellow-000 } | {: .bg-green-000 }
[Rocky Linux 9](rockylinux.md) | ? | ? | ? 
[Amazon Linux 2023](amazonlinux.md)| ? | ? | ? 
[VMware Photon OS 5.0](photon.md)| ? | ? | ? 
[Ubuntu LTS 24.04 (Jammy Jellyfish)](ubuntu.md)| ? | ? | ? 
[Debian 11 (bullseye)](debian.md)| ? | ? | ? 

<table>
  <tbody>
    <tr>
      <th>Distribution</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td>[SUSE Leap](leap.md)</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td>[Redhat Enterprise Linux 9 (RHEL)](rhel.md)</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td>[Redhat Enterprise Linux 8 (RHEL)](rhel.md)</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td>[CentOS Stream 9](centos.md)</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td>[CentOS Stream 8](centos.md)</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td>[CentOS 7](centos.md)</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;vertical-align:middle;text-align:center;" >Yes</td>
    </tr>
  </tbody>
</table>



## Details

Distribution| glibc Version | Package Manager | FileSystem
---|----|---|---
[SUSE Linux Enterprise Server (SLES)](https://www.suse.com/products/server/) | 2.31 | zypper | brtfs/ZFS
[SUSE Leap](leap.md) | 2.31 | zypper | brtfs/ZFS
[Redhat Enterprise Linux 9 (RHEL)](rhel.md)| 2.34 | yum 
[CentOS Stream 9](centos.md)| 2.34 | yum | 
[Rocky Linux 9](rockylinux.md)|2.34 | yum | https://rockylinux.org/
[Alma Linux 9](amalinux.md)|2.34|yum | https://almalinux.org
[Amazon Linux 2023](amazonlinux.md)|2.34 | yum | (fedora) https://aws.amazon.com/amazon-linux-2/
[Oracle Linux 9](oraclelinux.md)| 2.34 | yum | (fedora) https://www.oracle.com/linux/
[VMware Photon OS 5.0](photon.md)| 2.36 | yum | https://vmware.github.io/photon/
[Ubuntu LTS 24.04 (Jammy Jellyfish)](ubuntu.md) | 2.35 | apt | https://ubuntu.com/
[Debian 11 (bullseye)](debian.md)| 2.31 | apt 

## Resources

* [Domino Start Script](https://nashcom.github.io/domino-startscript/)
* [Domino on touch installer and installation step by step for CentOS Stream](https://nashcom.github.io/domino-startscript/install_domino/)


## Articles

* [Picking the right Linux Distribution](https://blog.nashcom.de/nashcomblog.nsf/dx/picking-the-right-linux-distribution.htm)
* [Taking a closer look at Linux distributions for NGINX, Curl and OpenSSL for Domino](https://blog.nashcom.de/nashcomblog.nsf/dx/taking-a-closer-look-at-linux-distributions-for-nginx-curl-and-openssl-for-domino-.htm)
* [ARM CPU platform -- Where can it be relevant today for you?](https://blog.nashcom.de/nashcomblog.nsf/dx/arm-cpu-platform-where-can-it-be-relevant-today-for-you.htm)


## Interesting links

https://microk8s.io/

## Wild and crazy 
A collection of non-standard environments that run HCL Domino

* [Pocket sized Domino server](https://blog.thomashampel.com/blog/tomcat2000.nsf/dx/domino-portable-edition-building-the-smallest-domino-server-hot-pants-for-geeks.htm)
* [QNAP Network Attached Storage](https://opensource.hcltechsw.com/domino-container/howto_qnap/)
