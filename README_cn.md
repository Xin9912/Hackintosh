# Hackintosh <br>
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;
## 神舟战神Z7M-KP7GT的黑苹果EFI文件
* 这是神舟战神Z7M-KP7GT的黑苹果安装文件。现在能够在macOS Bigsur11.4(OC的EFI)下使用, 如果你有和我相近的配置你可以进行尝试, 配置内容如下:

| 设备 | 型号 |
| ---- | ---- |
| 笔记本型号 |神舟战神Z7M-KP7GT |
| 主板 | 蓝天 N850HJ |
| CPU | Intel i7-7700HQ |
| 集显 | UHD630 |
| 独显 | Nvidia GTX 1050ti(已屏蔽) |
| 声卡 | ALC269VC |
| 无线网卡 | Brcm943224 | <br>

* **文件描述:** 本仓库中有EFI(基于OC-RELEASE编辑)~~及EFI-DEBUG(基于OC-DEBUG编辑)~~，如果你的笔记本是作为你的日常工作的工具，请尽量使用RELEASE版本的EFI，如果不是你可以自由选择。CLOVER引导的EFI在 仓库-发布里面，其版本是5112(在macOS10.15.5下工作良好，但是不保证其在10.15.6及以上版本能够正常使用)。

## 现在的问题
* 如果你的笔记本关机后再开机，在任意一个由本仓库EFI文件引导的系统你会发现，你上次的键盘背光设置已经被覆盖了。我不知道如何解决。 <br>
* DP输出不支持热拔插(如果你需要外接显示请保证笔记本是处于睡眠或者关机状态再接入dp线开启电脑)

## 更新日志 <br>
2021-11-13
<br>
* **1.** 更新至OC0.7.5
* **2.** 升级并添加一些Kexts
* **3.** 修复蓝牙在macOS12.0+无法使用(使用BlueToolFixup.kext)
-----
2021-7-11
<br>
* **1.** 更新至OC0.7.1
* **2.** 更新Kexts
-----
2021-5-11
<br>
* **1.** 更新至OC0.6.9
* **2.** 添加dp输出(请在关机前接入dp第一口)
* **3.** 更新Kexts
* **4.** 添加x86的电源管理
-----
2021-4-8
<br>
* **1.** 更新至OC0.6.8
* **2.** 更新Kexts
-----
2021-2-27
<br>
* **1.** 更新至OC0.6.6
* **2.** 更新Kexts
* **3.** 修改开机启动界面
-----
2021-2-1
<br>
* **1.** 更新至OC0.6.5
* **2.** 更新Kexts
* **3.** 修改SSDT-PNLF以保证在新版本opencore能够调节亮度
-----
2021-1-4
<br>
* **1.** 更新至OC0.6.4
* **2.** 删减并更新Kexts
* **3.** 删减部分ssdts
* **4.** 更新DEBUG版本(输出日志)
-----
2020-11-17
<br>
* **1.** 更新至OC0.6.3
* **2.** 优化电源管理
* **3.** 更新Kexts
* **4.** 添加Bigsur支持
* **5.** 重编译一些ssdts
-----
2020-10-06
<br>
* **1.** 更新至OC0.6.1
* **2.** 加入有线网卡驱动
* **3.** 更新Kexts
-----
 2020-8-28
<br>
* **1.** 加入CPU电源管理(通过加入CPUFriend及定制的CPUFriendDataProvider驱动)
* **2.** 替换启动页面主题(与原生白果相似)
* **3.** 替换PS2设备驱动(acidanthera版本)
* **4.** 在config.plist加入博通网卡的PCI路径(如果你的网卡不正常工作请加入自己网卡PCI路径)
* **5.** 屏蔽SDCard设备路径以节电(我也不知道有用不)


## 注意
* **1.** 我已经移除了关于SMBIOS的设置，请根据个人情况在config.plist添加信息。你应该修改 EFI_RELEASE(DEBUG)/OC/config.plist-PlatformInfo-Generic里的相关内容。(如果不修改其他系统可能会有问题)<br>
* **2.** 本仓库的文件都是经过自己的电脑测试的，但不免可能由于其他因素造成电脑的损伤，本人概不负责(也没有能力负责).
* **3.** 如果你需要在电脑上使用其他操作系统(除macOS&win)，请在config.plist里修改Scanpolicy的值.
* **4.** 请将你下载的版本文件夹名称(EFI_XXX)修改为EFI.
* **5.** 如果dp外接显示器无法使用, 请尝试下接入dp线睡眠或者重启电脑

## Kexts驱动版本

| 驱动名称 | 版本 |
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