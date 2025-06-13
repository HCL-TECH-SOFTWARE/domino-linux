---
layout: default
title: "Home"
nav_order: 1
description: "HCL Domino Linux"
has_children: true
---
<h1>Welcome</h1>
Documentation about how to run HCL Domino on the various Linux distributions.
This page is community supported and welcomes contributions.

<details close markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Background
The system requirements for HCL Domino include RHEL/CentOS and SUSE because those are the releases that HCL has tested (aka "certified") to run on. However, HCL Domino will run on other distributions if a certain minimum criteria is met. This repository is documenting which flavours of Linux customers have reported to be running HCL Domino on and what to be aware of.

## HCL Domino Compatibility
This table provides the collective knowledge of which distribution are known to be working with a Domino version.
Please note, only distributions declared as "Certified" are tested by HCL.

<table>
  <caption>HCL Domino on Linux Compatibility Matrix</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14.5</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
     <tr>
      <td><a href="linux/rhel">Redhat Enterprise Linux</a></td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
    </tr>
    <tr>
      <td><a href="linux/sles">SUSE Linux (SLES)</a></td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
    </tr>
    <tr>
      <td><a href="linux/amazonlinux">Amazon Linux</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/almalinux">Alma Linux</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/astralinux">Astra Linux</a></td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/centos">CentOS Stream</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/debian">Debian</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/opensuse">OpenSUSE</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/oracle">Oracle Linux</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/rockylinux">Rocky Linux</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/ubuntu">Ubuntu</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="linux/photon">VMware Photon OS 5.0</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
  </tbody>
</table>

### Experimental
Linux distributions in this chapter are rolling releases, so any compatibility statement can be obsolete by the time you are reading this document. Be careful, use at your own risk!

<table>
  <caption>HCL Domino on Linux Compatibility Matrix</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14.5</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td><a href="linux/archlinux">Arch Linux</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
    </tr>
    <tr>
      <td><a href="linux/fedora">Fedora</a></td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
    </tr>
    <tr>
      <td><a href="https://www.kali.org/">Kali Linux</a></td>
      <td style="background:#FFD147;text-align:center;" >Experimental</td>
      <td style="background:#FFD147;text-align:center;" >Experimental</td>
      <td style="background:#FFD147;text-align:center;" >Experimental</td>
      <td style="background:#FFD147;text-align:center;" >Experimental</td>
    </tr>
    <tr>
      <td><a href="linux/opensuse#opensuse-tubleweed">OpenSUSE Tumbleweed</a></td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
    </tr>
    <tr>
      <td><a href="https://github.com/wolfi-dev/">Wolfi OS</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
    </tr>
  </tbody>
</table>

### Definition

<table>
  <caption>Compatibility Definition</caption>
  <tbody>
    <tr>
      <th>Color</th>
      <th>Explanation</th>
    </tr>
    <tr>
      <td style="background:#00FF00" title="">Certified</td>
      <td>HCL has tested and supports this platform</td>
    </tr>
    <tr>
      <td style="background:#9EFF9E" title="">Yes</td>
      <td>Although not tested by HCL, seems to work just fine</td>
    </tr>
    <tr>
      <td style="background:#FFD147" title="">Limited</td>
      <td>May work with some some limitations. Use at your own risk</td>
    </tr>
    <tr>
      <td style="background:#FFC7C7" title="">No</td>
      <td>Has been tested and will not work</td>
    </tr>
    <tr>
      <td style="background:#C0C0C0" title="">Unknown</td>
      <td>Requires testing and may not be fully usuable</td>
    </tr>
  </tbody>
</table>

### Dependencies
Overview of HCL Domino dependencies

Domino Version | min. Kernel Version | min.glibc Version | min. stdc++ Version | Remarks
------| :---: | :---: | :---:
HCL Domino 14.5 | 5.14 | 2.34-28 | 11.2.1 | see [System Requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0108740)
HCL Domino 14.0.x | 5.14 | 2.34-28 | 11.2.1 | see [System Requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0108740)
HCL Domino 12.0.2 | 5.14 , 4.18 , 3.10.0-693 , 5.3.18 | ? | ? | see [System Requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0101447)
HCL Domino 11.0.x | ? | ? | ? | see [System Requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0102974)
HCL Domino 10.0.x | ? | ? | ? | see [System Requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0098707)
HCL Domino 9.0.1 FP10 | ? | ? | ? | see [System Requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0075441)


## Resources

* [Domino Start Script](https://nashcom.github.io/domino-startscript/)
* [Domino One Touch installer and installation step by step for CentOS Stream](https://nashcom.github.io/domino-startscript/install_domino/)

## Articles

* [What Is the Best Linux Distribution for HCL Domino?](https://blog.nashcom.de/nashcomblog.nsf/dx/what-is-the-best-linux-distribution-for-hcl-domino.htm)
* [Picking the right Linux Distribution](https://blog.nashcom.de/nashcomblog.nsf/dx/picking-the-right-linux-distribution.htm)
* [Taking a closer look at Linux distributions for NGINX, Curl and OpenSSL for Domino](https://blog.nashcom.de/nashcomblog.nsf/dx/taking-a-closer-look-at-linux-distributions-for-nginx-curl-and-openssl-for-domino-.htm)
* [ARM CPU platform -- Where can it be relevant today for you?](https://blog.nashcom.de/nashcomblog.nsf/dx/arm-cpu-platform-where-can-it-be-relevant-today-for-you.htm)


## Interesting links
* [Micro-Kubernetes](https://microk8s.io/)

## Wild and crazy 
A collection of non-standard environments that run HCL Domino

* [Pocket sized Domino server](https://blog.thomashampel.com/blog/tomcat2000.nsf/dx/domino-portable-edition-building-the-smallest-domino-server-hot-pants-for-geeks.htm)
* [QNAP Network Attached Storage](https://opensource.hcltechsw.com/domino-container/howto_qnap/)
