# Hackintosh
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;

## Descriptions <br>
* **Project:** It's EFI files to hackintosh for laptop Hasee Z7M-KP7GT. It may work well util macOS12.0.1. And if you have similar configurations to mine, you could try. And here is my laptop config: <br>
  
| Device | Model |
| ---- | ---- |
| Laptop model| Hasee Z7M-KP7GT |
| Motherboard| Clevo N850HJ |
| CPU | Intel i7-7700HQ |
| IGPU | UHD630 |
| DGPU | Nvidia GTX 1050ti(disabled)|
| Audio | ALC269VC |
| wireless card | Brcm943224 | <br>

* **Files:** The project provides EFI(based on release ocpkg) and ~~OC_DEBUG(based on debug ocpkg)~~. If you use your laptop in daily work, you'd better choose the release version, if not you could use one at will. And Clover is placed in the git repositories-release, the version is 5112(work well at macOS 10.15.5, may not work well at 10.15.6 and newer macOS version).  <br>

## What's Wrong <br>
* The keyboard backlight setting can't work if shutdown your laptop and then boot. And I don't know how to solve this problem. <br>
* Not support dp hot plug.(Please make sure your laptop is power off or asleep before you turn on it with dp output)<br>

## What's New <br>
2021-11-13
<br>
* **1.** Updated OC0.7.5
* **2.** Updated && Added Kexts
* **3.** Fixed Bluetooh in macOS12.0+(use BlueToolFixup.kext)
-----
2021-7-11
<br>
* **1.** Updated OC0.7.1
* **2.** Updated Kexts
-----
2021-5-11
<br>
* **1.** Updated OC0.6.9
* **2.** Supported dp output(please access dp connection before start)
* **3.** Updated Kexts
* **4.** Added x86 power management
-----
2021-4-8
<br>
* **1.** Updated OC0.6.8
* **2.** Updated Kexts
-----
2021-2-27
<br>
* **1.** Updated OC0.6.6
* **2.** Updated Kexts
* **3.** Modified boot theme
-----
2021-2-1
<br>
* **1.** Updated OC0.6.5
* **2.** Changed SSDT-PNLF.aml to make display could be adjustable in OC0.6.5
* **3.** Updated kexts
-----
2021-1-4
<br>
* **1.** Updated OC0.6.4
* **2.** Simplified ssdts
* **3.** Simplified&Updated kexts
* **4.** Updated DEBUG version
-----
2020-11-17
<br>
* **1.** Updated OC0.6.3
* **2.** Improved the power mangerment
* **3.** Updated kexts 
* **4.** Supported Bigsur
* **5.** Recomplied some ssdts
-----
2020-10-06
<br>
* **1.** Updated OC0.6.1
* **2.** Added wired lan kext 
* **3.** Updated kexts 
-----
 2020-8-28
<br>
* Added CPU power mangerment (CPUFriend and CPUFriendDataProvider kexts)
* Replaced boot theme (similar to original mac boot theme)
* Replaced PS2 device drivers (acidanthera version)
* Added Broadcom wireless card PCI path in config (you should add this if it not work well)
* Shielded SD Card PCI path to save power.(maybe useful and maybe not) 

## Attention <br>
* **1.** I removed SMBIOS settings in config.plist. So you should change them to your SMBIOS settings in EFI/OC/config.plist-PlatformInfo-Generic.(It may not work well on other OS if no those settings) <br> 
* **2.** I have tested all EFIs in my repository, and they work well . If your laptop works badly or some issues caused , I won't be responsible for them(I can't afford). <br>
* **3.** If you need Other OS(macOS&win excluded),you may need change the Scanpolicy vaule in config.plist(only support macOS and win now).
* **4.** You should change the name of the folder(EFI_XXX) downloaded and decompressed to EFI to make it work.
* **5.** If any display can't work, please sleep it and turn on it again.

## Kexts version <br>

| Name | Version |
| :----: | :----: |
| Lilu.kext| 1.5.7-RELEASE |
| VirtualSMC.kext| 1.2.7-RELEASE |
| WhateverGreen.kext | 1.5.5-RELEASE |
| ACPIBatteryManager.kext   | 1.90.1-RELEASE |
| AppleALC.kext | 1.6.6-RELEASE |
| AirportBrcmFixup.kext | 2.1.3-RELEASE |
| VoodooPS2Controller.kext | 2.2.7-RELEASE |
| RealtekRTL8111.kext   | 2.4.2-RELEASE |
| NVMeFix.kext	| 1.0.9-RELEASE |
<br>
