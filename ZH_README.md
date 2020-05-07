# archfi

这是一个简单，方便的bash脚本安装向导。

## 使用说明

在你下载并启动了Arch Linux镜像之后，进入命令行，就可以准备使用这个脚本了

通过这个脚本，你可以使用2种终端安装Arch Linux了。

这个脚本向导包括最小化安装包（Base, bootloader 还有可选的 archdi）
该脚本向导完成后, 你可以安装或启动 [archdi](https://github.com/MatMoul/archdi) (Arch Linux Desktop Install) 来安装和配置桌面环境.

这里提供了一个视频，方便查看如何使用它 [点这里](https://www.youtube.com/playlist?list=PLytHgIKLV1caHlCrcTSkm5OF2WSVI1_Sq).

## 使用用法

首先, 下载最新版Arch [最新版本镜像](https://www.archlinux.org/download/) 并且制作一个启动盘 [bootable device](https://wiki.archlinux.org/index.php/USB_flash_installation_media).
请确保在使用过程的网络环境，因为安装arch所需要的软件包，依赖于网络下载，如果你是用无线连接的，`wifi-menu`命令会有用处，当然你也可以阅读Arch Linux指南中的网络配置，了解更多详细说明
在命令行中输入下面的命令，下载该脚本:

    wget archfi.sf.net/archfi

如果 SourceForge 挂了, 用这个也行:

    wget matmoul.github.io/archfi

下载完后, 运行脚本:

    sh archfi

然后就可以一路根据向导完成安装系统了.

如果你需要更多的帮助, 请访问提供的视频内容，并按照内容进行操作.

## 更多自定义安装

    sh archfi -cpl {URL of your custom package list}

你可以在samples文件夹找到一个自定义包列表样本.

## 对于开发者

可以用下面命令测试脚本 :

    sh archfi -t {githubusername} {branchname}

举栗子 :

    sh archfi -t matmoul master
