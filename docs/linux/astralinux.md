---
layout: default
title: "Astra Linux"
parent: "Home"
nav_order: 4
description: "Astra Linux"
has_children: false
---
<h1>Alma Linux</h1>
[https://astralinux.ru/](https://astralinux.ru/)


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
| License         | Proprietary |
| Package Manager | dpkg |
| Filesystem      |    |
| Support         |   |
| Read more       | [Wikipedia: Astra Linux](https://en.wikipedia.org/wiki/Astra_Linux) |

## Compatibility

<table>
  <caption>HCL Domino compatibility with Astra Linux</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td><a href="#astra-linux">Common Edition</a></td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
     <tr>
      <td><a href="#astra-linux">Special Edition</a></td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
  </tbody>
</table>

## Versions
Which versions of this Linux distribution exists in the market and what HCL Domino version they are compatible with.

### Astra Linux Special Edition 

Commercial Linux distribution
### Astra Linux Common Edition

HCL Domino 11.0.1 {: .label .label-green }

Free Linux distribution, customers have successfully installed Domino. 

### What to be aware of

When adding a new user with adduser the -U option to create a matching group wasn't available but generating a group before with addgroup and using that group-id when creating the user via --gid worked as expected.

* The Domino installer will report the environment isn't supported.

* additional packages sysstat and gdb (GNU Debugger needed by NSD) may be useful

* NSH Start Script does not completely install automatically. The directory /etc/sysconfig is missing. Create an empty directory to fix it.

* NSD Debugging requires ptrace, which is disabled by default.
  * Check if ptrace lock is enabled:
  systemctl is-enabled astra-ptrace-lock
enabled
  * Disable ptrace lock: 
  astra-ptrace-lock disable
  * Check again that it is disabled:
systemctl is-enabled astra-ptrace-lock
disabled
  * Reboot the server for changes to take effect.

* Performance Tuning:
add "elevator=noop" to your grub kernel boot line using the graphical grub configuration. To check the settings use

cat /sys/block/sda/queue/scheduler
[noop] deadline cfq


For more details see
* [HCL Domino on Astralinux](https://blog.nashcom.de/nashcomblog.nsf/dx/domino-on-astra-linux-feedback.htm?opendocument) by Daniel Nashed


## References
* [HCL Domino on Astralinux](https://blog.nashcom.de/nashcomblog.nsf/dx/domino-on-astra-linux-feedback.htm?opendocument) by Daniel Nashed

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