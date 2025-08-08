---
{"dg-publish":true,"permalink":"/魔法教程/翻墙软件Nekobox详细使用教程/","updated":"2025-08-08T15:44:07.004+08:00"}
---


> 本文介绍了安卓代理软件Nekobox的下载与使用，你也可以选择直接跳转到[下载与安装的部分](#下载安装Nekobox)

## Nekobox介绍
==此段可以跳过==
Nekobox完整名字是NekoBox for Android，是一款使用 sing-box 的 Android 通用代理软件。也就是通常说的翻墙软件或者魔法软件。其中sing-box是其使用的核心。
Nekobox开源地址:https://github.com/MatsuriDayo/NekoBoxForAndroid
Nekobox官方文档:https://matsuridayo.github.io/
Nekobox支持以下协议的节点，部分协议需要安装插件后实现支持:

| 协议名称          | 支持情况 | 协议名称      | 支持情况 | 协议名称         | 支持情况                      |
| ------------- | ---- | --------- | ---- | ------------ | ------------------------- |
| SOCKS(4/4a/5) | 默认支持 | Trojan    | 默认支持 | Hysteria 1/2 | 默认支持                      |
| HTTP(S)       | 默认支持 | VLESS     | 默认支持 | WireGuard    | 默认支持                      |
| SSH           | 默认支持 | AnyTLS    | 默认支持 | Trojan-Go    | 需要插件:<br>trojan-go-plugin |
| Shadowsocks   | 默认支持 | ShadowTLS | 默认支持 | NaïveProxy   | 需要插件:<br>naive-plugin     |
| VMess         | 默认支持 | TUIC      | 默认支持 | Mieru        | 需要插件:<br>mieru-plugin     |


## 下载安装Nekobox
==下面的教程中提供的软件版本为教程编辑时的最新版本，不保证为查看教程时的最新版本==
用手机浏览器扫描二维码或打开下面的链接，又或者是用手机自带的扫描器扫描二维码均可跳转到下载。
Nekobox下载:https://github.com/MatsuriDayo/NekoBoxForAndroid/releases/download/1.3.9/NekoBox-1.3.9-arm64-v8a.apk
二维码:
![翻墙软件Nekobox详细使用教程-1.png|131](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-1.png)

*如果你的安卓设备不是传统的arm架构或者是老旧的32位arm架构，请参考下载正确版本*:
- arm架构老旧的安卓手机
	- https://github.com/MatsuriDayo/NekoBoxForAndroid/releases/download/1.3.9/NekoBox-1.3.9-armeabi-v7a.apk
	- ![翻墙软件Nekobox详细使用教程-2.png|131](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-2.png)
- x86架构的电脑设备和平板设备使用的
	- https://github.com/MatsuriDayo/NekoBoxForAndroid/releases/download/1.3.9/NekoBox-1.3.9-x86.apk
	- ![翻墙软件Nekobox详细使用教程-3.png|131](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-3.png)
- x86架构64位的电脑设备和平板设备使用的
	- https://github.com/MatsuriDayo/NekoBoxForAndroid/releases/download/1.3.9/NekoBox-1.3.9-x86_64.apk
	- ![翻墙软件Nekobox详细使用教程-4.png|131](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-4.png)

打开链接之后下载就会开始，等待下载完成安装即可。
## Nekobox使用
刚刚安装完成的Nekobox是没有任何的订阅和节点的，需要你自己导入。导入节点或者是导入订阅之后再选择一个合适的节点就可以开启代理了。
### 首次运行
当你安装完成Nekobox之后，首次打开将会提示你是否运行显示通知，点允许即可，否则你可能无法在手机通知栏看到当前的代理状态。
![翻墙软件Nekobox详细使用教程-5.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-5.webp)
### 导入节点
导入节点有两种方法，其中一种是通过剪贴板导入节点，还有一种是扫描二维码导入，二维码的内容本质是也是一个节点链接。
如何判断一个链接是否是节点链接:
节点链接不是`http`或者`https`开头的，如果你得到的是一个`http`或`https`开头的链接那么大概率那是一个订阅链接，请参考后面[[#导入订阅]]的步骤操作。
首先复制你的节点订阅，然后来到Nekobox中，点击右上角的 `+` 图标，选择`从剪贴板导入`，选择后你就会在主界面看到你导入的节点，如果提示成功后不显示，则退出软件并杀掉后台后重新进入就能看到。
![翻墙软件Nekobox详细使用教程-6.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-6.webp)

如果你手上有一个节点二维码，那么点击右上角的`+`图标，然后选择`扫描二维码`软件就会自动打开相机，对准二维码扫描就可以把节点添加进来。
如果你手机已经保存了那张二维码，那么扫描界面右上角点击之后就可以选择图片扫描二维码。
![翻墙软件Nekobox详细使用教程-7.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-7.webp)
### 导入订阅
如果你手上有一个链接是`http`或者`https`开头的。那么大概率是订阅链接，你可以按照下面的步骤添加到软件中并更新。
复制你的链接之后，点击软件左上方三条横杠的图标，选择`分组`，到分组页面之后点击右上角四条杠和一个加号的图标添加分组。
![翻墙软件Nekobox详细使用教程-8.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-8.webp)

在新建分组页面中，点击`分组名`，输入一个名字，用于区别不同的订阅，例如`订阅1`，点击确定。
然后点击分组类型选择订阅，当你把分组类型改成订阅之后，下面就会出现订阅链接的选项，点击订阅链接并粘贴你复制的链接进去。最后点击右上角的✔完成新建分组的设置。
![翻墙软件Nekobox详细使用教程-9.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-9.webp)

点击✔后软件就会自动开始更新订阅，稍等片刻之后就能看到更新成功的提示，下方会提示你更新的信息，列表中能看到最后一次更新的时间和手动更新的按钮。点击左上角三条杠选择`配置`，在配置页面就能看到多了一个标签，标签的名字就是刚刚设置的`订阅1`，点击标签就能看到订阅更新的节点。
![翻墙软件Nekobox详细使用教程-10.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-10.webp)
### 切换节点和开启代理
在主界面点击任意一个节点即可切换节点，当前选中的节点最左边会有竖线标识，选中节点后点击下方的圆形纸飞机图标即可开启代理。首次开启会提示添加网络链接请求，点击同意。然后手机下方就会出现当前的连接状态栏，点击状态栏就可以测试当前节点的延迟。
![翻墙软件Nekobox详细使用教程-11.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-11.webp)
### 批量测试延迟
点击右上角三个点，选择`TCPing`，等待测试完成，就能在每个节点最左边看到测试结果了，通常有数字代表节点可连通(可能可用)，但是如果显示超时(Timeout)那么节点肯定不可用。
![翻墙软件Nekobox详细使用教程-12.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-12.webp)

### 分应用代理
==要想让这个功能生效需要重新开启一遍代理，点击圆形按钮关闭，之后再点击圆形按钮开启==
当开启代理之后你可能会发现一些国内的软件速度缓慢，甚至是无法加载，这是因为软件默认把所有应用的流量都通过代理节点转发。想解决这个问题，你需要分应用代理功能。
点击右上角三条杠，点击`设置`，下滑找到`分应用代理`，点击右边的开关开启功能，点击之后页面就会跳转到应用选择页面。默认是`绕过`模式，也就是说下面被选择的应用将不会被转发到节点，而是直接连接的模式。这样例如微信等国内软件就不会收到翻墙软件的影响了。
选择完成之后点击左上角的`X`然后返回主界面，重新开启代理之后就会生效了。
![翻墙软件Nekobox详细使用教程-13.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-13.webp)

在上面的例子中可以看到，分应用代理页面中还有几个功能，他们分别是:
- `关闭` - `代理` - `绕过`
	- 这是设置当前分应用代理的模式。
	- `关闭` - 不开启分应用代理，默认全局模式。
	- `代理` - 下方选中的应用使用魔法，其他应用直连。
	- `绕过` - 下方选中的应用不使用魔法，其他使用魔法。
- `显示系统应用`
	- 手机系统自带的软件和组件可能不显示在下面的列表中，开启这个功能后就会显示。
- `自动选择需要代理的应用`
	- 由软件自动帮你选择一遍，当手机内软件过多的时候可以用这个功能初始化，然后再根据自己的需要修改。

![翻墙软件Nekobox详细使用教程-14.jpg](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-14.jpg)

### 路由规则
==要想让这个功能生效需要重新开启一遍代理，点击圆形按钮关闭，之后再点击圆形按钮开启==
当你开启代理之后，使用浏览器或者其他软件浏览一些网页会发现打不开了，这可能是因为:
1. 国内的服务不向国外用户提供，所以开启代理后打不开。
2. 访问的网站不在代理规则内，所以开启代理后打不开。
这个时候你可以自己手动添加规则来解决:
点击左上角三条杠，点击`路由`，再点击右上角的三条竖线添加一条路由规则:
![翻墙软件Nekobox详细使用教程-15.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-15.webp)

在新建路由规则界面，主要有三项需要设置:
- 路由名称
	- 这一条规则的名字，自行设置
- domain
	- 你需要代理的网站域名，通常你访问的网站都不是网站的顶级域名，你可以复制完整的网址到下面这个网站提取顶级域名部分。
	- https://seo.juziseo.com/tools/domain/
- outbound
	- 这个域名的流量需要如何处理，有下面几种模式:
		- 代理 - 通过节点访问
		- 绕过 - 不通过节点访问，直连
		- 屏蔽 - 直接不访问，通常用于屏蔽广告
![翻墙软件Nekobox详细使用教程-16.webp](/img/user/%E9%AD%94%E6%B3%95%E6%95%99%E7%A8%8B/pic/%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6Nekobox%E8%AF%A6%E7%BB%86%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B-16.webp)

