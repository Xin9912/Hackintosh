# Hackintosh
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;
## Descriptions <br>
* **Project:** It's EFI files to hackintosh for laptop Hasee Z7M-KP7GT. It may work well util macOS(Catalina)10.15.6. And if you have similar configurations to mine, you could try. And here is my laptop config: <br>

| Devices | Model |
| ---- | ---- |
| Laptop model| Hasee Z7M-KP7GT |
| Motherboard| Clevo N850HJ |
| CPU | Intel i7-7700HQ |
| IGPU | UHD630 |
| DGPU | Nvidia GTX 1050ti(disabled)|
| Audio | ALC269VC |
| wireless card | Brcm943224 | <br>

* **Files:** The project provide OC_RELEASE EFI(based on release ocpkg) and OC_DEBUG(based on debug ockg). If you use your laptop in daily work, you'd better choose the release version, if not you could use one at will. And Clover is placed in the git project-release, the version is 5112(work well at macOS 10.15.5, may not work well at 10.15.6 and newer macOS version).  <br>

## What's Wrong <br>
* **1.** The laptop OC version is newer than OC0.5.8 may wake later than using OC0.5.8 if you want to use after it sleeped. I have try some ways to solve the prolem, but it have no use at all. And you can try your way.  <br>
* **2.** The keyboard blacklight setting can't work if shutdown your laptop and then boot. And I don't know how to sovle this problem. <br>

## What's New <br>
* Added CPU mangerment(CPUFriend and CPUFriendDataProvider kexts)
* Replaced themes(similar to original mac boot theme)
* Replaced PS2 device drivers(acidanthera version rather than rehubman)
* Added Broadcom wireless card PCI path in config(you should add this if it not work well)
* Shielded SD Card PCI path to save power.

## Attention <br>
* **Note**:I removed SMBIOS settings in config.plist. So you should change them to your own SMBIOS settings in EFI/OC/config.plist-PlatformInfo-Generic. <br>

| Bootloader | macOS version |
| ---- | ---- |
| Opencore 0.5.8 Realease | macOS Catalina 10.15.5 |
|Clover 5112 (Stop Updating) | macOS Catalina 10.15.5 |
