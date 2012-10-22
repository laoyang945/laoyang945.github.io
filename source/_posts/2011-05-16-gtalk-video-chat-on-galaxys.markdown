---
layout: post
title: '三星i9000实现gtalk视频/语音聊天'
date: 2011-5-16
wordpress-id: gtalk-video-chat-on-galaxys
comments: true
---
Android 2.3.4发布估计最大的亮点就是实现了手机上面的Gtalk视频聊天了，但是，现在官方升级到2.3.4的就只有亲儿子NEXUS S。广大其他手机用户纷纷表示愤慨，于是在XDA上有这么<a href="http://forum.xda-developers.com/showthread.php?t=1056793">一个39页的帖子</a>在讨论如何将NEXUS S上面的google talk提取出来，让其他型号的也能用上。

这个替代方法的关键就在于下载正确的Google Apps包。不能下载http://goo-inside.me/gapps/里提供的（他的gtalk在关闭对话的时候有bug，大小也不对），也不能只用1.3M的Talk.apk去替换已经有的talk.apk。必须将整个googleserviceframework以及相关文件都添加并替换。

完全文件打包在这里：<a href="http://freakshare.com/files/blgrh5us/gapps-gb-20110503-signed.zip.html" target="_blank">http://freakshare.com/files/blgrh5us/gapps-gb-20110503-signed.zip.html</a>

你也可以试试这个（xda上另一个人给的，我没试）：<a href="http://www.mediafire.com/?92475r3frlncg29" target="_blank">http://www.mediafire.com/?92475r3frlncg29</a>

下载后放在SD卡上，进入恢复模式安装即可

如果你是用的CM7最新版本，那么恭喜你，刷了这个包之后你的Google Talk就可以双向视频/音频聊天了（所谓双向，是指能从电脑呼叫手机、也能从手机呼叫电脑），而且用的是前置摄像头

如果你用的是LIDROID的2.4，双向聊天是可以的，但是采用的是后置摄像头

Juwe的ROM也是只能用后置摄像头

DarkyRom没有测试，欢迎留言分享测试结果

使用效果：语音很流畅（缺点是从扬声器出声、最好用耳机），视频也可以，我和大连的 @coolcfan还有我澳大利亚的同学测试了都不卡。不过分辨率是惨点……

另外，关于最近访问Gmail的问题，似乎用hosts文件将www.google.com，webcache.googleusercontent.com，www.google.com.hk和mail.google.com都指向北京谷歌公司的IP203.208.39.22即可暂时解决。

注：

goo-inside.me的解释如下：

<strong>So what's up with the 2.3.4 GApps?</strong>

This is a tricky one. The problem here is that Google, unlike what they've done for every previous update to the G1, Nexus One, Nexus S, etc., decided to compile the Talk2.apk and libtalk_jni.so to be compatible only with the neon board, and ARM v7 (aka, the Nexus S), rather than every board, the
actual Gingerbread API's, and ARM v6 and Tegra as well. So here's where this leaves us:
