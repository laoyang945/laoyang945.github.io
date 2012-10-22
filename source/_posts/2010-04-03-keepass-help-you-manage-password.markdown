---
layout: post
title: 'Keepass帮你管理密码'
date: 2010-4-3
wordpress-id: keepass-help-you-manage-password
comments: true
---
在网络上注册的服务是越来越多了，虽然有时候可以用Google帐号或者Twitter帐号来使用，但是这样的网站还是不多，多数网站仍然要你自己创建一个帐户。在帐号和密码的管理上，大概有这么几种形式：
<ul>
	<li>多帐号同密码：非常不安全，只要攻破一个帐户拿到密码就相当于把你的邮箱也破掉了。</li>
	<li>多帐号多密码，密码按安全要求分级：相对更好，安全性取决于密码的强度。</li>
</ul>
今天推荐一个密码管理软件<a href="http://keepass.info/" target="_blank">Keepass</a>，它能够帮你生成安全性很高的随机密码并对各个网站的密码进行管理，对我来说显得更方便的是<strong>，Keepass有对应的Firefox扩展和黑莓手机客户端！</strong>
<h4>下载及安装</h4>
这个软件的使用就很简单了，在<a title="http://keepass.info/download.html" href="http://keepass.info/download.html">http://keepass.info/download.html</a>下载1.17版本或者2.10版本（两者的不同在于后者需要.Net框架或者Mono），下载可选择安装版或便携版，我下载的是1.17便携版本。

同时在下载页面上还可以看到有多种手机平台的客户端下载

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image.png"><img style="display: inline; border-width: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb.png" border="0" alt="image" width="484" height="304" /></a>

作为一个黑莓玩家，显然会下载黑莓版本的客户端，下载地址在<a title="http://f5bbutils.fairview5.com/keepassbb/download/" href="http://f5bbutils.fairview5.com/keepassbb/download/">http://f5bbutils.fairview5.com/keepassbb/download/</a>，选最新版本的zip包下载，解压之后用DM或者将cod+jad文件拷贝到手机上安装。
<h4>桌面端</h4>
运行之后选择新建一个数据库，输入并确认新数据库的管理密码，Keepass会提示你密码的强度如何，在新建的时候可以选择一个文件作为钥匙，这样以后打开数据库的时候除了密码还需要那个钥匙文件：

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image1.png"><img style="display: inline; border-width: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb1.png" border="0" alt="image" width="484" height="372" /></a>

主界面上左边是树状目录，右边显示详情：

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image2.png"><img style="display: inline; border-width: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb2.png" border="0" alt="image" width="484" height="372" /></a>

新建密码，点击“Add Entry”即可，需要注意的是那个Title设置是很有用的，他可以帮助Keepass在自动填表的时候识别目标网址或者程序。密码可以输入或者随机生成。添加完成后别忘了点保存保存数据文件（.kdb格式）。

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image3.png"><img style="display: inline; border: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb3.png" border="0" alt="image" width="483" height="535" /></a>

Keepass能够自动填表，比如我新建一个标题为“豆瓣”的项目，URL也填写豆瓣的

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image4.png"><img style="display: inline; border: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb4.png" border="0" alt="image" width="484" height="138" /></a>

以后只要在Keepass开启的情况下，打开豆瓣网的首页，光标定位到Email，按下Ctrl+Alt+A（如果QQ在Keepass之前运行这个全局快捷键就会失效）就能自动输入Keepass中保存的这一条目。除了在网页上，在应用软件中也可以自动填表，支持包括MSN,QQ等很多软件。

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image5.png"><img style="display: inline; border: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb5.png" border="0" alt="image" width="484" height="164" /></a>

需要注意的是，如果从Keepass拷贝内容（用户名，密码）到剪贴板的话，是有时间限制的：

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/image6.png"><img style="display: inline; border-width: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/04/image_thumb6.png" border="0" alt="image" width="407" height="36" /></a>
<h4>Firefox扩展</h4>
一个名叫<a href="http://keefox.org/" target="_blank">KeeFox</a>的项目，使得Firefox和Keepass能够整合到一起，但是目前还是在开发期。同时它只支持2.x以上的Keepass。我这里没有测试，感兴趣的读者可以参考<a href="http://api.postrank.com/log?url=http%3A%2F%2Fplaypcesor.blogspot.com%2F2010%2F03%2Fkeefox-keepass-firefox.html">KeeFox 將 KeePass 密碼管理軟體整合進 Firefox 當中</a>这篇文章。
<h4>黑莓端</h4>
安装完成后，Keepass就会出现在你的桌面，操作比较简单，看图不说话～

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113153.png"><img style="display: inline; border: 0px;" title="20100403113153" src="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113153_thumb.png" border="0" alt="20100403113153" width="324" height="244" /></a>

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113202.png"><img style="display: inline; border: 0px;" title="20100403113202" src="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113202_thumb.png" border="0" alt="20100403113202" width="324" height="244" /></a>

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113217.png"><img style="display: inline; border: 0px;" title="20100403113217" src="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113217_thumb.png" border="0" alt="20100403113217" width="324" height="244" /></a>

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113227.png"><img style="display: inline; border: 0px;" title="20100403113227" src="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113227_thumb.png" border="0" alt="20100403113227" width="324" height="244" /></a>

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113258.png"><img style="display: inline; border: 0px;" title="20100403113258" src="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113258_thumb.png" border="0" alt="20100403113258" width="324" height="244" /></a>

<a href="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113310.png"><img style="display: inline; border: 0px;" title="20100403113310" src="http://laoyang.info/blog/wp-content/uploads/2010/04/20100403113310_thumb.png" border="0" alt="20100403113310" width="324" height="244" /></a>

其实黑莓也自带密码管理器，但是电脑上的密码很难一个一个的输入手机，所以我觉得Keepass会显得方便～。我现在两台电脑的kdb文件用的是<a href="http://www.dropbox.com" target="_blank">dropbox</a>来同步，手机可以访问m.dropbox.com来下载kdb文件。

最后有一个小小的请求，如果读者有还没有开始使用<a href="http://www.dropbox.com" target="_blank">dropbox</a>的，可以通过<a title="https://www.dropbox.com/referrals/NTEwNjA1OTY5" href="https://www.dropbox.com/referrals/NTEwNjA1OTY5">https://www.dropbox.com/referrals/NTEwNjA1OTY5</a> 这个链接注册并下载程序使用一次，这样我们的容量都能增加。
