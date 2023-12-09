---
layout: default
title: "RedHat Enterprise Server"
parent: "Home"
nav_order: 9
description: "RedHat Enterprise Server"
has_children: false
---
<h1>RedHat Enterprise Server</h1>
[https://www.redhat.com/](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux/server)

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
| License         |    |
| Package Manager | yum |
| Filesystem      |    |
| Based on        |    |
| Support         |    |
| Read more       | [Wikipedia: RedHat Enterprise Linux](https://en.wikipedia.org/wiki/Red_Hat_Enterprise_Linux) |

## Versions
Which versions of this Linux distribution exists in the market and what HCL Domino version they are compatible with.

### RHEL 9

Library | Version
---|---
kernel | 5.14
glibc  | 2.34-28
libstdc++ | 11.2.1

HCL Domino 14.0
{: .label .label-green }


### RHEL 8

HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }


### RHEL 7

HCL Domino 14.0
{: .label .label-red }

### RHEL 6

HCL Domino 14.0
{: .label .label-red }

## Compatibility
Item | Compatibility
---| ---
Linux StartScript | Yes/No/Tested/Certified


<table>
  <caption>HCL Domino on Linux Compatibility Matrix</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td><a href="rhel">Redhat Enterprise Linux 9</a></td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="rhel">Redhat Enterprise Linux 8</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
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
      <td>Will work with some tuning</td>
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

## References

* [Redhat Linux for up to 16 machines](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux)
* [No-cost Red Hat Enterprise Linux Individual Developer Subscription](https://developers.redhat.com/articles/faqs-no-cost-red-hat-enterprise-linux)
* [Easier ways to access RHEL](https://www.redhat.com/en/blog/new-year-new-red-hat-enterprise-linux-programs-easier-ways-access-rhel)
* [Redhat Developer Portal](https://developers.redhat.com/)
