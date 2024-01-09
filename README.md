# MagicBook-16-Pro-Sonoma-EFI

 荣耀 MagicBook 16 Pro (HYM-WXX) 锐龙版 黑苹果 EFI 文件

➡️ [点我查看设备详情](https://www.hihonor.com/cn/laptops/magicbook-16-pro/)

### 配置信息
- CPU：AMD Ryzen 7 5800H with Radeon Graphics
- RAM：16GB DDR4
- GPU0：NVIDIA Geforce RTX 3050 Laptop
> NVIDIA 显卡无法在 macOS 10.14+ 上驱动
- GPU1：AMD Radeon Grphics（集显）
- 网卡：Qualcomm QCNFA765
> 无法驱动，详情请见 [后面](https://github.com/SoraSushi776/MagicBook-16-Pro-Sonoma-EFI#%E8%B5%84%E6%96%99%E9%93%BE%E6%8E%A5)

### 伪装信息
- 型号：MacBook Pro 16,3
> MacBook Pro (13-inch, 2020, Two Thunderbolt 3 ports)
- 伪装CPU：Intel Core i7 8557U
- 伪装显卡：Iris Plus Graphics 645

### 已知问题
- 第一组 Type-C 和 USB 接口（位于两个接口上面靠近显示器的那两个）无法使用，插入设备开机会卡死（未解）
> 一个 Type-C 和 USB 组成一组集线器，第一组集线器不能工作，第二组可以工作。建议使用 [AMDTools](https://github.com/SoraSushi776/MagicBook-16-Pro-Sonoma-EFI#%E8%B5%84%E6%96%99%E9%93%BE%E6%8E%A5) 将第一组屏蔽
- 显存需要使用 [AMDTools]() 修改成 4G（或其它）
- 内置网卡无法驱动，解决方法请看 [后面](https://github.com/SoraSushi776/MagicBook-16-Pro-Sonoma-EFI#%E8%B5%84%E6%96%99%E9%93%BE%E6%8E%A5)

### 关于网卡

由于内置网卡没有办法驱动，目前唯一解决方案是 **购买使用外置网卡**，并搭配 [Github]() 上的一个驱动进行使用，本EFI已内置Kext驱动，只需要安装其软件即可

我用的是 [COMFAST CF-811AC](http://www.comfast.cn/index.php?m=content&c=index&a=show&catid=13&id=74)

**请注意！官网上的驱动不支持 macOS 11.0 及以后版本！请使用 [Github]() 上提供的驱动**

本EFI已解决内建网卡问题，Apple ID 服务 和 App Store 均可访问

### 其他想说的
- 建议使用恢复镜像方法安装系统，使用引导安装不保证能成功
- 如果你安装Ventura/Sonoma的时候卡死，可以先装一次Big Sur（反正我就是先装一次Big Sur就好了）
- 直到进入桌面前，都建议将 NootedRed.kext 关闭（Sonoma必须关闭）

### 资料链接
- AMDTools：https://github.com/DavidS95/Smokeless_UMAF
- 外置网卡驱动安装与教程：https://imacos.top/2021/02/19/0519/