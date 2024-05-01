---
title: Product Guide - GPU Passthrough
description: Instructions for host and guest configuration to use GPU passthrough
published: true
date: 2023-06-26T12:29:19.096Z
tags: 
editor: markdown
dateCreated: 2023-03-27T19:53:35.522Z
---

# GPU Passthrough

<br>
<br>

## Host Installation/Configuration

> VergeIO includes the driver for generic PCI address passthrough; typically, no additional host drivers are needed for GPU passthrough. {.is-info}

1.  From the Main Dashboard, click **Nodes**.
2.  Click **Drivers** on the left menu.
3.  Click **New** on the left menu.

![ledunsupported.png](/public/userguide-sshots/newdriverpassthru.png)


4.  Select ***node*** from the dropdown list.
5.  Select ***VFIO-PCI Passthrough*** in the ***Driver*** dropdown list.
6.  Check/select all display controller PCI devices to be used for GPU passthrough, in the ***Apply to PCI Devices*** section.
7.  Click **Submit** at the bottom of the page.


<br>
<br>


## Guest Configuration

1.  **Power down the VM**.
2.  Navigate to the **dashboard of the desired VM** (From the main dashboard click **Machines** on the left menu, **Virtual Machines**, **double-click desired VM** in the listing.)
3.  Click **Devices** on the left menu.
4.  Click **New** on the left menu. The Device Entry Form appears.

![ledunsupported.png](/public/userguide-sshots/gpunewdeviceform.png)

5.  Optionally, a ***Name*** and ***Description*** can be entered for the device.
6.  Select **GPU Passthrough** in the ***Type*** dropdown list.
7.  ***UUID*** is a universally unique identifier and is persistent across reboots. Typically UUID should be left blank to allow the system to automatically assign one to the device; a specific UUID can be entered if necessary (e.g. imported or cloned VMs with existing GPU PCI device).
8.  Click **Submit** at the bottom of the page.
9.  **Power on the VM**.
10.  **Install appropriate guest driver**. Required guest driver(s) will depend on specific GPU hardware and guest OS version. Consult your GPU hardware documentation for guidance.

<br>   

> Need more Help? Email <a href="mailto:support@verge.io?subject=Support Inquiry" target="_blank" rel="noopener noreferrer">support@verge.io</a> or call us at <a href="tel:+855-855-8300">(855) 855-8300</a>{.is-info}

<br>

<div style="text-align:center; margin-bottom:5px">
  <a href="../ProductGuide/menu"><button class="button-grey"><b>↺</b> Back to the Product Guide</button></a>
  <a href="https://www.verge.io/test-drive#Demo-Section"><button class="button-cta">🚗 Take a Test Drive Today!</button></a>
</div>