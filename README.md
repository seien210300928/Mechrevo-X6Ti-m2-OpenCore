# Mechrevo-X6Ti-m2-OpenCore

## 软件说明
本OC引导基于[OpenCore-0.9.9](https://github.com/acidanthera/OpenCorePkg)与[Mechrevo-X6Ti-OpenCore](https://github.com/YuZhangWang/Mechrevo-X6Ti-OpenCore)制作,不保证兼容其他类似机型
自带
Monterey的蜂窝网络驱动为[AirportItwm](https://github.com/OpenIntelWireless/itlwm/)，安装完成即可使用
BigSur与Catalina的蜂窝网络驱动为[Itwm](https://github.com/OpenIntelWireless/itlwm/)，需要配合[Macsoftward](./Macsoftward)文件夹中的[HeliPort](https://github.com/OpenIntelWireless/HeliPort)应用使用

## 文件夹内容说明
- [Macsoftward](./Macsoftward)为安装和调试黑苹果可能会用到的Mac软件
- [Winsoftward](./Winsoftward/)为安装和调试黑苹果可能会用到的Mac软件
- [Monterey](./Mechrevo-X6Ti-m2-OpenCore/Monterey/)为安装BigSur所需引导OC
- [BigSur](./Mechrevo-X6Ti-m2-OpenCore/BigSur/)为安装BigSur所需引导OC
- [Catalina](./Mechrevo-X6Ti-m2-OpenCore/Catalina/)为安装Catalina所需引导OC
- [Mechrevo-X6Ti-m2-OpenCore-v](./Mechrevo-X6Ti-m2-OpenCore-v/)为安装此机型-v模式的OC引导

## 安装步骤
1. 使用任意的可引导镜像文件将MacOS安装器刻录进您的移动磁盘设备
- 如果您使用的是官方的不可引导镜像文件刻录，请将刻录好的移动磁盘设备新建一个ESP分区
2. 将移动磁盘设备中的ESP分区的EFI文件夹删除，替换为相应版本的EFI文件
3. 现在您就可以使用移动磁盘设备中的OpenCore引导开始安装MacOS了 
4. 进入安装好的MacOS
5. 使用OpenCore Configurator挂载MacOS所在磁盘和移动磁盘设备的EPS分区
6. 将MacOS所在磁盘的EPS分区中的EFI文件夹删除，替换为移动磁盘设备中的ESP分区的EFI文件夹

## 后续
未知原因，Monterey系统无法识别MacOS所在硬盘以外的其他磁盘，本人也在寻找原因，求助大神

因为硬件限制，本人无力制作此机型的Sonoma(MacOS14)与Ventura(MacOS13)的OC引导文件

## 提示
说明中的非原本仓库软件超链接均可点击直达原仓库