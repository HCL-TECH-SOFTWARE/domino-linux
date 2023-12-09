---
layout: default
title: "Installation"
nav_order: 2
description: "Installation"
has_children: false
---

<h1>Installation Methods</h1>
Installing HCL Domino on Linux can be done in different ways

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Before you start
* Check the system requirements
* Update Linux 
* The following will be used:
```
User : notes
Group: notes
Binary Directory: /opt/hcl/domino
Data Directory  : /local/notesdata
```

## Manual installation

* To start the Domino installer, you must be root

```
sudo su
./install
```

{% include yewtube.html id="fW1iPlcoDSo" %}
* [Install Domino Server on Linux Environment](https://yewtu.be/watch?v=fW1iPlcoDSo)

For more information, see [online help](https://help.hcltechsw.com/domino/14.0.0/admin/inst_installingdominoonunixsystems_t.html)


## Scripted Installation

Probably the easiest and fastest way to install a HCL Domino server is to use an installation script, e.g. the one provided by Daniel in the [Domino-StartScript repository](https://github.com/nashcom/domino-startscript)

```
curl -sL https://raw.githubusercontent.com/nashcom/domino-startscript/main/install_domino.sh | bash -
```

### GUI Installation

## Nash!Com Start-script



