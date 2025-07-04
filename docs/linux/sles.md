---
layout: default
title: "SUSE Linux Enterprise Server"
parent: "Home"
nav_order: 12
description: "SUSE Linux Enterprise Server"
has_children: false
---

<h1>SUSE Linux Enterprise Server (SLES)</h1>
[https://www.suse.com/products/server/](https://www.suse.com/products/server/)

<details close markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Overview

| --- | --- |
| Certified by HCL | Yes |
| License         |  GPL |
| Package Manager | zypper |
| Filesystem      | [brtfs](../filesystems.md#btrfs), ZFS |
| Based on        |    |
| Support         |    |
| Read more       | [Wikipedia: SUSE Linux](https://en.wikipedia.org/wiki/SUSE_Linux) |
| Download        | [Evaluation Copy](https://www.suse.com/download/sles/) |


## Compatibility

<table>
  <caption>HCL Domino compatibility with SUSE Linux</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14.5</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
 <tr>
      <td><a href="#suse-linux-enterprise-15-sp6">SUSE Linux (SLES) 15 SP6</a></td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#FFD147;text-align:center;" >Maybe</td>
    </tr> <tr>
      <td><a href="#suse-linux-enterprise-15-sp3">SUSE Linux (SLES) 15 SP3</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
    </tr>
    <tr>
      <td><a href="#suse-linux-enterprise-12">SUSE Linux (SLES) 12.x</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
    </tr>
  </tbody>
</table>

## Versions
Which versions of this Linux distribution exists in the market and what HCL Domino version they are compatible with.
### SUSE Linux Enterprise 15 SP6

HCL Domino 14.5
{: .label .label-green }
HCL Domino 14.0
{: .label .label-green }
HCL Domino 12.0.2
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-yellow }

Customers have reported Domino 14 + 12.0.2 to run on SLES 15 SP6, but HCL has not certified this version yet.
For Domino 11.0.1 no information exist

* [SUSE Linux Enterprise Server 15 SP6 Release Notes](https://documentation.suse.com/en-us/sles/15-SP6/)

### SUSE Linux Enterprise 15 SP3

HCL Domino 14.5
{: .label .label-red }
HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.2
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

{: .warning }
HCL Domino 14 requires glibc to be provided in a specific version which SUSE Linux 15 SP3 does not provide. SLES 15sp6 provides glibc in the required version but has not been fully tested yet.

Domino 12.0.2 and 11.0.1 are certified on SLES 15 SP3 (with kernel 5.3) for details see [Domino 12.0.2 System Requirements ](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0101447)

### SUSE Linux Enterprise 12

HCL Domino 14.5
{: .label .label-red }
HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.2
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

{: .warning }
HCL Domino 14 requires glibc to be provided in a specific version which SUSE Linux 12 does not provide.

## References

* [OpenSUSE](opensuse.md) Leap is a distribution similar to SLES but free of charge.

## Definition

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