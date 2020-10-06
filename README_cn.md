# Hackintosh <br>
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;
## 神舟战神Z7M-KP7GT的黑苹果EFI文件
* 这是神舟战神Z7M-KP7GT的黑苹果安装文件。现在能够在macOS10.15.7(OC的EFI)下使用, 如果你有和我相近的配置你可以进行尝试, 配置内容如下:

| 设备 | 型号 |
| ---- | ---- |
| 笔记本型号 |神舟战神Z7M-KP7GT |
| 主板 | 蓝天 N850HJ |
| CPU | Intel i7-7700HQ |
| 集显 | UHD630 |
| 独显 | Nvidia GTX 1050ti(已屏蔽) |
| 声卡 | ALC269VC |
| 无线网卡 | Brcm943224 | <br>

* **文件描述:** 本仓库中有EFI-RELEASE(基于OC-RELEASE编辑)及EFI-DEBUG(基于OC-DEBUG编辑)，如果你的笔记本是作为你的日常工作的工具，请尽量使用RELEASE版本的EFI，如果不是你可以自由选择。CLOVER引导的EFI在 仓库-发布里面，其版本是5112(在macOS10.15.5下工作良好，但是不保证其在10.15.6及以上版本能够正常使用)。

## 现在的问题
* ~~~ **1.** 如果你使用的本仓库的OC版本高于OC0.5.8版本你可能会发现，当你将笔记本睡眠后重新打开再唤醒会出现唤醒比OC0.5.8唤醒慢的问题。我尝试果许多方法，但是并没有什么作用，你可以按照你的方法尝试一下解决这个问题。如果你解决好了，请麻烦你分享一下。 <br>~~~
* **2.** 如果你的笔记本关机后再开机，在任意一个由本仓库EFI文件引导的系统你会发现，你上次的键盘背光设置已经被覆盖了。我不知道如何解决。 <br>

## 更新日志 <br>
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
* **1.** 我已经移除了关于SMBIOS的设置，请根据个人情况在config.plist添加信息。你应该修改 EFI_RELEASE(DEBUG)/OC/config.plist-PlatformInfo-Generic 里的相关内容。<br>
* **2.** 本仓库的文件都是经过自己的电脑测试的，但不免可能由于其他因素造成电脑的损伤，本人概不负责(也没有能力负责).

## Kexts驱动版本

| 驱动名称 | 版本 |
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
