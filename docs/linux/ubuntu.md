---
layout: default
title: "Ubuntu Linux"
parent: "Home"
nav_order: 13
description: "Ubuntu Linux"
has_children: false
---

<h1>Ubuntu Linux</h1>
[https://ubuntu.com/](https://ubuntu.com/)

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
| Package Manager | apt |
| Filesystem      |  |
| Based on        | [Debian](debian.md)  |
| Support         |    |
| Read more       | [Wikipedia: Ubuntux](https://en.wikipedia.org/wiki/Ubuntu) |

## Compatibility

<table>
  <caption>HCL Domino compatibility with SUSE Linux</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td><a href="#ubuntu-2204-lts-jammy-jellyfish">Ubuntu 22.04 (Jammy Jellyfish)</a></td>
      <td style="background:#FFD147;text-align:center;" >Kernel 6.x</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
  </tbody>
</table>


## Versions
Which versions of this Linux distribution exists in the market and what HCL Domino version they are compatible with.
### Ubuntu 22.04 LTS (Jammy Jellyfish)

HCL Domino 14.0
{: .label .label-yellow }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

{: .attention }
Ubuntu introduced a new major 6.x kernel option in 22.04-03 LTS. This kernel is not supported by Domino 14 yet, so downgrading to Kernel 5.x is required.

The following information is based on this blog post from Daniel Nashed

The 6.x kernel installation depends on the Hardware enablement stack (HWE).
By default the HWE package is only installed on Desktops, but some providers might have already switched to the later kernel.

The Ubuntu LTS enablement, or Hardware Enablement (HWE), stack provides the newer kernel and X support for existing Ubuntu LTS releases. That stack can be enabled manually, but may also be pre-enabled with an Ubuntu LTS release.

For details check the [Lifecycle document](https://ubuntu.com/kernel/lifecycle).

Once this HWE package is installed, Ubuntu supports the 6.x kernel which will be then installed by default.

#### Enable Boot Menu

Make sure to have boot console access to the server and see how the boot menu looks like. In some cases the boot menu might be hidden and needs to be enabled first. e.g. If it is hidden with **GRUB_TIMEOUT_STYLE=hidden** and a timeout for the boot menu set to 0 seconds. 

Enable the boot menu via:

```
vi /etc/default/grub

GRUB_TIMEOUT_STYLE=countdown
GRUB_TIMEOUT=10

update-grub
```


#### Hardware Enablement Stack (HWE)

Check if Hardware Enablement Stack (HWE) is enabled by querying the status:

```
hwe-support-status --verbose

You are not running a system with a Hardware Enablement Stack. Your system is supported until April 2027
```

If enabled, querying the status will return just this message:
```
hwe-support-status --verbose

Your Hardware Enablement Stack (HWE) is supported until April 2027.
```

**Disable Hardware Enablement Stack (HWE)**

If HWE is installed, remove it to avoid future kernel updates to a 6.x kernel.
Note, this doesn't remove the newer kernel. It just removes the HWE package.

```
apt-get remove linux-generic-hwe-22.04
apt autoremove
```

#### Query installed kernels

To check if an older kernel is still installed by running the following command:

```
apt list --installed | grep linux-image

linux-image-5.15.0-91-generic/jammy-updates,jammy-security,now 5.15.0-91.101 amd64 [installed,automatic]
linux-image-6.2.0-39-generic/jammy-updates,jammy-security,now 6.2.0-39.40~22.04.1 amd64 [installed,automatic]
```

#### Install a 5.x kernel

In the example above, a 5.15 kernel is already installed.
If not, then install it manually with the following command:

```
apt-get install --install-recommends linux-image-5.15.0-91-generic
```

**Switch to the 5.x kernel from the boot menu**

During boot count down press `ESC` and select the advanced menu if the **5.x kernel** is not listed in the main menu.

Once the new kernel is installed, reboot and switch to the 5.x kernel from the boot menu. Note, it is not possible to remove a running kernel that was booted from.

**Verify**

Check if the the kernel 5.x is active using the following command:

```
uname -a
Linux ubuntu-4gb-nbg1-1 5.15.0-91-generic #101-Ubuntu SMP Tue Nov 14 13:30:08 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
```

#### Remove the 6.2 kernel

Check if kernel 6.x is listed earlier and remove it. The grub menu should be automatically updated:

```
apt-get remove linux-image-6.2.0-39-generic
```

Finally reboot and check if the machine still boots up.


## References

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