---
layout: default
title: "RedHat Enterprise Server"
parent: "Home"
nav_order: 10
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
| Certified by HCL | Yes |
| License         |    |
| Package Manager | yum |
| Filesystem      |    |
| Based on        |    |
| Support         | [Red Hat Enterprise Linux Life Cycle](https://access.redhat.com/support/policy/updates/errata#Extended_Life_Cycle_Phase) |
| Read more       | [Wikipedia: RedHat Enterprise Linux](https://en.wikipedia.org/wiki/Red_Hat_Enterprise_Linux) |

## Compatibility

<table>
  <caption>HCL Domino on RHEL Linux Compatibility Matrix</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td><a href="#rhel-10">Redhat Enterprise Linux 10</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="#rhel-9">Redhat Enterprise Linux 9</a></td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="#rhel-8">Redhat Enterprise Linux 8</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
      <td style="background:#00FF00;text-align:center;" >Certified</td>
    </tr>
  </tbody>
</table>

## Versions
Which versions of this Linux distribution exists in the market and what HCL Domino version they are compatible with.

### RHEL 10

HCL Domino 14.5
{: .label .label-green }
HCL Domino 14.0
{: .label .label-green }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

RHEL 10 has been released after Domino 14.0 shipped, so it has not (yet) been undergoing the certification tests at HCL, however, customers have reported it to work fine.

[Standard installation methods](../installation.md) apply.

### RHEL 9
HCL Domino 14.5
{: .label .label-green }
HCL Domino 14.0
{: .label .label-green }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

Works fine. [Standard installation methods](../installation.md) apply.

### RHEL 8
HCL Domino 14.5
{: .label .label-red }
HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

Please note the end of support statement from Red Hat:
* [Red Hat Enterprise Linux Life Cycle](https://access.redhat.com/support/policy/updates/errata#Extended_Life_Cycle_Phase)

This version of RHEL does not provide the required kernel version for Domino 14.0 and higher to work.

### RHEL 7

{: .warning }
RHEL 7 has reached its end of mainstream support / end of marketing and should not be used any longer. Extended support may be provided by RedHat. For details see [RHEL 7 end of maintenance](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux/rhel-7-end-of-maintenance)

for RHEL 7.4+ :

HCL Domino 14.5
{: .label .label-red }
HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

This version of RHEL does not provide the required kernel version for Domino 14.0 and higher to work.

### RHEL 6
{: .warning }
RHEL 7 has reached its end of life and end of extended support on 30. June 2024 and should not be used any longer. 

HCL Domino 14.5
{: .label .label-red }
HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

This version of RHEL does not provide the required kernel version for Domino 14.0 and higher to work.
## References

* [Red Hat Linux for up to 16 machines](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux)
* [No-cost Red Hat Enterprise Linux Individual Developer Subscription](https://developers.redhat.com/articles/faqs-no-cost-red-hat-enterprise-linux)
* [Easier ways to access RHEL](https://www.redhat.com/en/blog/new-year-new-red-hat-enterprise-linux-programs-easier-ways-access-rhel)
* [Red Hat Developer Portal](https://developers.redhat.com/)
* [Red Hat Enterprise Linux Life Cycle](https://access.redhat.com/support/policy/updates/errata#Extended_Life_Cycle_Phase)

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