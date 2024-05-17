---
title: UEFI Tweaks for Imported VMs
slug: uefi-tweaks-for-imported-vms
description: Addressing UEFI Devices on Imported VMs
published: true
date: 2023-01-24T14:15:45.862Z
categories:
  - VM
  - Troubleshooting
tags: vm, import, uefi, secure boot
editor: markdown
dateCreated: 2022-06-28T14:46:35.084Z
---

## UEFI disks as boot devices will not boot properly  

After importing VM images leveraging UEFI disks as boot devices, sometimes the VM will not boot properly inside the VergeIO platform.  To resolve this, tweaks to boot order/options need to be made.


Here is a list of suggested solutions for issues with imported VMs not booting because of guest UEFI bios settings:

### Solution 1

1. From a fresh import of the VM (before trying to power it up inside VergeIO), edit the VM in Verge and enable the UEFI boot option.
2. Power on the VM
3. Hit ESC within 5 seconds to get into the VM BIOS (you can edit the VM settings in Verge to increase the boot timer if necessary)
4. Enter the BIOS and navigate to Boot Manager options (varies by bios)
5. Change the selected boot device to the Verge IO device
6. Exit the UEFI BIOS
7. Reboot the VM 

### Solution 2

1. From a fresh import of the VM (before trying to power it up inside VergeIO), edit the VM in Verge and enable the UEFI boot option.
1. Power on the VM
1. Hit ESC within 5 seconds to get into the VM BIOS (you can edit the VM settings in Verge to increase the boot timer if necessary)
1. Enter the BIOS and navigate to Boot Manager options (varies by bios)
1. Disable secure boot as an option
1. Exit the UEFI BIOS
1. Reboot the VM 
<br>

> Need more Help? Email <a href="mailto:support@verge.io?subject=Support Inquiry" target="_blank" rel="noopener noreferrer">support@verge.io</a> or call us at <a href="tel:+855-855-8300">(855) 855-8300</a>{.is-info}

<br>
<div style="text-align: center">
  <a href="https://wiki.verge.io/en/public/kb"><button class="button-grey"> <b>↺</b> Back to Knowledgebase</button></a>
<a href="https://www.verge.io/test-drive"><button class="button-orange">🚗 Take a Test Drive Today!</button></a>
</div>