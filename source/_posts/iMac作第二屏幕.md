title: iMac作第二屏幕
date: 2015-01-26 15:36:49
tags: [Mac, 双屏]
photos: [/img/imac-dual-screen.jpg, /img/thunderbolt.png]
---

虽然[这里](http://news.zol.com.cn/article/364051.html)提供了iPad作为第二屏幕的做法，但实测效率太低，屏幕也太小，起码满足不了我对大屏的需求。
iMac屏幕够大，必要时给Mac Air作为第二屏幕也是不错的选择。这里使用了官方提供的[Target Display](http://support.apple.com/kb/PH4469)方法。

#### 步骤
1. 准备双端Thunderbolt接口的电缆（淘宝即可，官方比较贵）
1. 使用Thunderbolt连接任意两台Mac设备
1. 假如iMac当作第二屏幕，则在iMac键盘上键入Command(⌘)-F2
1. 退出TD模式，在键盘上键入同样按键即可

#### 问题
1. 进入TD模式后，iMac的外置设备（键盘、鼠标等）不能用了。
官方没有说明，我摸索出来的方法如下：
	* iMac上启用*Screen Sharing*，记录下vnc地址
	* Mac Air连接该vnc地址，禁用iMac的*Bluetooth*
	* 打开Mac Air的*Bluetooth*，与外置键盘、鼠标等配对

1. TD模式下拔出Thunderbolt，iMac会一直假死。
暂时无解，似乎只能长按关机键了。。。
