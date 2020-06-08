# Hackintosh
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;
## Descriptions <br>
* It's EFI files to hackintosh for laptop Hasee Z7M-KP7GT. It may work well util macOS(Catalina)10.15.5. And if you have similar configurations to mine, you could try it.Well, here is my laptop config: <br>

| Devices | Model |
| ---- | ---- |
| Laptop model| Hasee Z7M-KP7GT |
| Motherboard|HM175 series |
| CPU | Intel i7-7700HQ |
| IGPU | UHD630 |
| DGPU | Nvidia GTX 1050ti|
| Audio | ALC269VC |
| wireless card | Brcm943224 |

## What's Wrong <br>
* Well, I got a perfect EFI with bootloaded Opencore 0.5.8 Release(enable DGPU,so I disable dgpu-off.aml), and I my laptop's **Graphics/Display** have something suprising, I will show you the photo as follow.So, could you driver it on my laptop? <br>
![Wrong Graphics/Displays](https://images.gitee.com/uploads/images/2020/0608/141442_7dee4853_5740238.png "屏幕截图.png")

## Attention <br>
* I have configured OC and it works well on my laptop. I think I will use opencore to boot system rather than Clover. <br>
* Clover works well on my laptop, but the keyboard blacklight setting can't work if shutdown your laptop and then boot. <br>
* **Note**:I removed SMBIOS settings in config.plist. So you should change the SMBIOS settings in the config.plist which you choose. <br>

| Bootloader | macOS version |
| ---- | ---- |
| Opencore 0.5.8 Realease | macOS Catalina 10.15.5 |
|Clover 5118 (Stop Updating) | macOS Catalina 10.15.5 |
