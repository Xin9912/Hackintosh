# Hackintosh
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;

## Descriptions <br>
* **Project:** It's EFI files to hackintosh for laptop Hasee Z7M-KP7GT. It may work well util macOS(Catalina)10.15.7. And if you have similar configurations to mine, you could try. And here is my laptop config: <br>
  
| Device | Model |
| ---- | ---- |
| Laptop model| Hasee Z7M-KP7GT |
| Motherboard| Clevo N850HJ |
| CPU | Intel i7-7700HQ |
| IGPU | UHD630 |
| DGPU | Nvidia GTX 1050ti(disabled)|
| Audio | ALC269VC |
| wireless card | Brcm943224 | <br>

* **Files:** The project provides OC_RELEASE EFI(based on release ocpkg) and OC_DEBUG(based on debug ocpkg). If you use your laptop in daily work, you'd better choose the release version, if not you could use one at will. And Clover is placed in the git repositories-release, the version is 5112(work well at macOS 10.15.5, may not work well at 10.15.6 and newer macOS version).  <br>

## What's Wrong <br>
* ~~**1.** The laptop OC version is newer than OC0.5.8 may wake later than using OC0.5.8 if you want to use it after it slept. I have tried some ways to solve the problem, but it has no use at all. And you can try your way.~~  <br>
* **2.** The keyboard backlight setting can't work if shutdown your laptop and then boot. And I don't know how to solve this problem. <br>

## What's New <br>
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
* **1.** I removed SMBIOS settings in config.plist. So you should change them to your SMBIOS settings in EFI/OC/config.plist-PlatformInfo-Generic. <br> 
* **2.** I have tested all EFIs in my repository, and they work well. If your laptop works badly or some issues caused , I won't be responsible for them(I can't afford). <br>

## Kexts version <br>

| Name | Version |
| :----: | :----: |
| Lilu.kext| 1.4.7-RELEASE |
| VirtualSMC.kext| 1.1.6-RELEASE |
| WhateverGreen.kext | 1.4.2-RELEASE |
| AppleALC.kext | 1.5.1-RELEASE |
| AirportBrcmFixup.kext | 2.0.8-RELEASE |
| VoodooPS2Controller.kext | 2.1.6-RELEASE |
| NoTouchID.kext | 1.0.3-RELEASE |
| CPUFriend.kext | 1.2.1-RELEASE | 
| RealtekRTL8111.kext | 2.2.2-RELEASE | <br>
