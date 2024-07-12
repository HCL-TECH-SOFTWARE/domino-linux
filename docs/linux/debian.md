---
layout: default
title: "Debian"
parent: "Home"
nav_order: 5
description: "Debian"
has_children: false
---
<h1>Debian</h1>
[https://www.debian.org](https://www.debian.org/)

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
| Certified by HCL | No |
| License         | Free Open Source, DFSG |
| Package Manager | apt |
| Filesystem      |    |
| Based on        |    |
| Support         |    |
| Read more       | [Wikipedia: Debian](https://en.wikipedia.org/wiki/Debian) |

## Overview

<table>
  <caption>HCL Domino compatibility with Debian</caption>
  <tbody>
    <tr>
      <th>Linux Distribution</th>
      <th>Domino 14</th>
      <th>Domino 12</th>
      <th>Domino 11</th>
    </tr>
    <tr>
      <td><a href="#debian-12-bookworm">Debian 12 (bookworm)</a></td>
      <td style="background:#9EFF9E;text-align:center;" >Kernel 6.x</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
    <tr>
      <td><a href="#debian-12-bullseye">Debian 11 (bullseye)</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
      <td style="background:#9EFF9E;text-align:center;" >Yes</td>
    </tr>
      <tr>
      <td><a href="#debian-12-buster">Debian 10 (buster)</a></td>
      <td style="background:#FFC7C7;text-align:center;" >No</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
      <td style="background:#C0C0C0;text-align:center;" >Unknown</td>
    </tr>
  </tbody>
</table>

## Versions
Which versions of this Linux distribution exists in the market and what HCL Domino version they are compatible with.

### Debian 12 Bookworm

HCL Domino 14.0
{: .label .label-green }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

### Debian 11 Bullseye

HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

Kernel version does not allow to run HCL Domino 14

### Debian 10 Buster

HCL Domino 14.0
{: .label .label-red }
HCL Domino 12.0.x
{: .label .label-green }
HCL Domino 11.0.1
{: .label .label-green }

Kernel version does not allow to run HCL Domino 14

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