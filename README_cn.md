# Hackintosh <br>
* [English](https://github.com/Xin9912/Hackintosh/blob/master/README.md)
* [简体中文](https://github.com/Xin9912/Hackintosh/blob/master/README_cn.md)
&emsp;
## 神舟战神Z7M-KP7GT的黑苹果EFI文件
* 这是神舟战神Z7M-KP7GT的黑苹果安装文件。现在能够在macOS10.15.6(Catalina)下使用, 如果你有和我相近的配置你可以进行尝试, 配置内容如下:

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
* **1.** 如果你使用的本仓库的OC版本高于OC0.5.8版本你可能会发现，当你将笔记本睡眠后重新打开再唤醒会出现唤醒比OC0.5.8唤醒慢的问题。我尝试果许多方法，但是并没有什么作用，你可以按照你的方法尝试一下解决这个问题。如果你解决好了，请麻烦你分享一下。 <br>
* **2.** 如果你的笔记本关机后再开机，在任意一个由本仓库EFI文件引导的系统你会发现，你上次的键盘背光设置已经被覆盖了。我不知道如何解决。 <br>

## 注意
* 我现在已经配置好了Opencore 0.5.8Realease，在我的笔记本上运行很好。我想我以后应该会使用Opencore而不再是Clover了。<br>
* Clover现在可以完美引导macOS10.15.4, 不过电脑硬重启后键盘背光不会被保存下来，可以添加一下补丁修复即可。
* **注意**: 我已经移除了关于OC及Clover的关于SMBIOS的设置，请根据个人情况在config.plist添加信息。<br>

| 引导工具 | 支持的macOS版本 |
| ---- | ---- |
| Opencore 0.5.8 Realease | macOS Catalina 10.15.5 |
|Clover 5112 (停止更新) | macOS Catalina 10.15.5 |

