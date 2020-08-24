# Hackintosh
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;
## Descriptions <br>
* **Project:** It's EFI files to hackintosh for laptop Hasee Z7M-KP7GT. It may work well util macOS(Catalina)10.15.6. And if you have similar configurations to mine, you could try. And here is my laptop config: <br>

| Devices | Model |
| ---- | ---- |
| Laptop model| Hasee Z7M-KP7GT |
| Motherboard| Clevo HM175 series |
| CPU | Intel i7-7700HQ |
| IGPU | UHD630 |
| DGPU | Nvidia GTX 1050ti(disabled)|
| Audio | ALC269VC |
| wireless card | Brcm943224 | <br>

* **Files:** The project provide OC_RELEASE EFI(based on release ocpkg) and OC_DEBUG(based on debug ockg). If you use your laptop in daily work, you'd better choose the release version, if not you could use one at will.And Clover is placed in the git project-release, the version is 5112(work well at macOS 10.15.5, I am not sure it work well at 10.15.6).  <br>

* **What's

## What's New <br>
* The keyboard blacklight setting can't work if shutdown your laptop and then boot.

## Attention <br>
* I have configured OC and it works well on my laptop. I think I will use opencore to boot system rather than Clover. <br>
* Clover works well on my laptop, but  <br>
* **Note**:I removed SMBIOS settings in config.plist. So you should change or set the SMBIOS settings in the config.plist which you choose. <br>

| Bootloader | macOS version |
| ---- | ---- |
| Opencore 0.5.8 Realease | macOS Catalina 10.15.5 |
|Clover 5112 (Stop Updating) | macOS Catalina 10.15.5 |
