<div align="center">
 
<img alt="LOGO" src="https://github.com/Inter1006/PenPointOS_Vbox/blob/Readme_Files/logo.svg" width="300" height="100" />
 
# PenPointOS -Emulator-
在 VirtualBox 上运行的 PenPoint 操作系统~<br />

[![LICENSE](https://img.shields.io/badge/LICENSE-Apache2.0-green.svg?style=for-the-badge)](https://github.com/Inter1006/PenPointOS_Vbox/blob/main/LICENSE )

</div>

## 📝关于这个项目
本项目为一个仿真实例，旨在让PenPointOS在虚拟机中正常启动，并搭配其SDK及编译器，在现代平台上复现PenPoint的软件开发环境。<br />
为了保证兼容性和令系统正常启动，我们选择了FreeDOS作为启动PenPoint的前置操作系统，并使用VirtualBox作为虚拟机平台。

## 📚本项目包含的内容

* FreeDOS 1.3-rc4(官网[freedos.org](https://www.freedos.org/))
* 一个可运行的PenPoint OS 1.0a 副本
* PenPoint OS 1.x Update3
* PenPoint OS SDK工具&Developer Utilities(来源:[Bitsavers](http://www.bitsavers.org/bits/Go/PENPOINT_SDK/))
* WATCOM 9.1 Compiler(编译工具,其后继者为[OpenWatcom](https://www.openwatcom.org/))
* PenPoint程序开发示例作品(已编译好并预装在系统内，源代码见`PENPOINT\SDK\SAMPLE`
* 一些PenPoint软件(已预装在系统内)

## 📥如何安装?
1.下载VirtualBox并安装好。<br />
 （VirtualBox官方网站:https://www.virtualbox.org/ ）<br />
2.下载本存储库提供的 **.ova** (开放虚拟机格式)文件,该文件可以在[发行版本](https://github.com/Inter1006/PenPointOS_Vbox/releases)中找到。<br />
3.双击下载好的.ova文件，这应该会启动VirtualBox，如果你做对了前面几步，VirtualBox应该会弹出"导入虚拟电脑"的窗口。<br />
4.在弹出的窗口中点击 **完成(F)** 即可。稍等片刻，名为"PenPoint OS 1.0a Update3"的虚拟机将会出现在VirtualBox管理器左侧的列表中。
## ❓如何启动PenPoint?
1.在**VirtualBox管理器**<img alt="PICTURE" src="https://github.com/Inter1006/PenPointOS_Vbox/blob/Readme_Files/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-07-10%20193523.png" width="200" height="20" />左侧的列表中找到你导入的虚拟电脑(导入方法见上面)。<br />
2.在管理器窗口右侧单击 **启动(T)**<img alt="PICTURE" src="https://github.com/Inter1006/PenPointOS_Vbox/blob/Readme_Files/START.svg" width="20" height="20" />。<br />
3.等待虚拟电脑启动，直到其显示"Loading Completed"字样并启动到 C:\ 提示符。<br />
4.输入 **GO** ，回车即可。
## 🛠️进阶教程Chapter1-为PenPoint OS安装软件
Chapter 1:安装已有软件<br />
PenPoint OS使用带有“QINSTALL"标识文件的软盘安装应用程序。如果你连接了一张QINSTALL软盘，系统会自动识别并打开软件包管理器。<br />
详细步骤如下(附上Dock栏参考图):![屏幕截图 2024-06-22 115831](https://github.com/Inter1006/PenPointOS_Vbox/assets/86058148/17c3ebf0-1329-4727-8936-61e50f40c265)<br />

1.插入一张QINSTLL软件盘到虚拟软驱中(如果有多张软盘则插入第一张)。<br />
2.等待系统识别软盘，如果没有自动识别则双击Connections(Dock栏从左数第三个图标)，不出意外的话系统会打开下图所示的Quick Installer窗口(这里使用GOFax安装盘做演示)。<br />

怎么样？看到最右侧Install那一列的选框了吗？单击选框即可安装，安装成功后选框会打上对号表示安装成功(注意，部分依赖文件，如上图的“Install Me First"软件，安装成功后也不会打上对勾。）<br />

至此，软件包的安装便结束了。如果安装软件的过程中提示”Insert Disk xxx“，按照序号换盘即可。安装完成后，你便可以关闭Quick Installer和Connections窗口，弹出软盘了。<br />

## 🛠️进阶教程Chapter2-Debug Version与串口调试
敬请期待-Coming soon....

## ❗注意事项
有时PenPoint OS会拒绝启动，对此，你可以将调试日志重定向到串行日志。<br />
若要这样做，请编辑 `\PENPOINT\BOOT\MIL.INI`，并取消注释 `SerialDebugPort=l` 和 `#LowLevelDebug=com1` 这两行代码。<br />
其他问题等待补充.....

## ℹ关于
作者:
<table>
  <tr>
    <td align="center"><a href="https://github.com/Inter1006"><img src="https://github.com/Inter1006/PenPointOS_Vbox/blob/Readme_Files/b_fa517952f054ca8c99a234cc1b50b50b.jpg" width="100px;" alt=""/><br /><sub><b>INTER_INIT</b></sub></a><br /></td>
  </tr>
</table>

特别感谢[Kirill Leyfer](https://github.com/BOOtak),他总结了PenPointOS在现代虚拟硬件上启动的前置条件。

[作者的b站个人主页](https://space.bilibili.com/1756824708)<br />
qq交流群:**981893945** 欢迎来玩

## 🤝友站链接
[351workshop官网](https://www.351workshop.top/)<br />
👆点击戳一下WNT351<br />
[樱之谷-MC服务器](www.sakuravalley.xyz)<br />
👆点击戳一下Axium. 钰




