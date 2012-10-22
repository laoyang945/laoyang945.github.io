---
layout: post
title: '如何用Kindle看RSS'
date: 2011-1-25
wordpress-id: kindle-rss
comments: true
---
每天的阅读任务除了书、论文还有Google Reader，前两者在大多数情况下可以用我的Kindle DXG完成，那Google Reader也可以在Kindle上看吗？当然可以，而且方法不止一种。

（因为DXG只有3G这一种联网方式，所以没法像KINDLE3一样在wifi下通过@free.kindle.com这个账户来接收RSS，操作上只能将RSS的打包文件下载到电脑然后传到KINDLE上，多了一个步骤）
### 浏览器直接访问Google Reader
从Kindle自带浏览器访问http://www.google.com/reader/m 访问GR的手机版即可，当然，速度可能很慢，也有可能连不上（视你所在地区的3G信号而定）

<img src="https://lh6.googleusercontent.com/_W7vzKfSkTVE/TT6aY_j06oI/AAAAAAAAEfI/psiSb8q6BDE/s512/screen_shot-12178.png" alt="" />

<span style="color: #888888;">网络不好的时候无法访问，不能离线阅读</span>

和用手机访问Google Reader一样，可以完成加星标、分享等功能，读过的条目也在GR里面标记为已读

<img class="picasa" src="https://lh4.googleusercontent.com/_W7vzKfSkTVE/TT6aZCc1aHI/AAAAAAAAEfM/lkPGlVhC4oM/s512/screen_shot-12179.png" alt="" /><!--more-->

<img class="picasa" src="https://lh3.googleusercontent.com/_W7vzKfSkTVE/TT6aj6WBB1I/AAAAAAAAEfU/27bQQNbE4pQ/s512/screen_shot-12180.png" alt="" />

<img class="picasa" src="https://lh6.googleusercontent.com/_W7vzKfSkTVE/TT6aj5OcyWI/AAAAAAAAEfY/VWmTgOBXGLw/s512/screen_shot-12182.png" alt="" />

<span style="color: #888888;">包含Google Reader大多数功能，除了"like"</span>
### 通过Feedbooks无线下载
可惜的是，我才没用几天，这个服务就暂停了……

<img class="picasa" src="https://lh6.googleusercontent.com/_W7vzKfSkTVE/TT6aYkCFqHI/AAAAAAAAEe8/hP_oEVmRUNU/s512/2011-01-25%2016%2058%2041.png" alt="" />
### 通过KindleReader
网址是http://reader.dogear.mobi/，过对这个应用授权后，可以定时将Google Reader中的未读文章打包发送到你的free.kindle.com邮箱（K3好像在wifi下可以无限投递），可以指定分类打包，也可以将已发送的文章标记为已读，另外，kindlereader还提供一个在线阅读的功能（测试中），依然存在网络延迟影响阅读体验。

<img class="picasa" src="https://lh6.googleusercontent.com/_W7vzKfSkTVE/TT6aY2bs77I/AAAAAAAAEfA/N46elhxrnBw/s512/2011-01-25%2017%2001%2029.png" alt="" />

<span style="color: #888888;">kindleReader设置蛮简单的</span>

<img class="picasa" src="https://lh5.googleusercontent.com/_W7vzKfSkTVE/TT6aY1A3UyI/AAAAAAAAEfE/KhBPdhXzwmQ/s512/2011-01-25%2017%2003%2004.png" alt="" />

<span style="color: #888888;">对DXG，会收到一封包含下载链接的信，将那个azw文件传到Kindle上即可</span><span style="color: #888888;">，似乎K3可以在wifi下直接无线传递到机器上？</span>

<img src="https://lh3.googleusercontent.com/_W7vzKfSkTVE/TT6apzU9kdI/AAAAAAAAEfw/G5-c7ZwV23A/s512/screen_shot-12194.png" alt="" />

<span style="color: #888888;">注意，图没了</span>

<img class="picasa" src="https://lh4.googleusercontent.com/_W7vzKfSkTVE/TT6akJS9ruI/AAAAAAAAEfc/izNysyHS07k/s512/screen_shot-12188.png" alt="" />

<span style="color: #888888;">这是在线版的KindleReader</span>

<img class="picasa" src="https://lh5.googleusercontent.com/_W7vzKfSkTVE/TT6akL32qCI/AAAAAAAAEfg/5-Q1rCgsfIw/s512/screen_shot-12191.png" alt="" />

<span style="color: #888888;">有图有真相</span>

kindlereader转换后图片丢失（在线阅读可以看到，不过如果遇到防盗链那也没辙）

kindlereader的另一个特点是它是一个开源应用，可以将它架设在自己的服务器（GAE是可以的）上。项目地址在https://bitbucket.org/jiedan/kindlereader，教程在<a href="http://iapp.tk/2010/12/google-gae-rss-to-kindle/" target="_blank">http://iapp.tk/2010/12/google-gae-rss-to-kindle/</a>
### 通过Kindlefeeder
kindlefeeder网址是http://www.kindlefeeder.com，是一个将RSS转换为Kindle可读格式的服务，免费用户可以添加12个feed（不过你知道世界上有种东西叫做yahoo pipes，而且google reader里面的分类设置为公开之后也可以直接订阅）

使用方式大同小异，不过Kindlefeeder的mobi文件下载，定时投递，无限feed这三个功能只对付费用户开放，一年20美元。

Kindlefeeder给你的RSS没有图片

<img class="picasa" src="https://lh5.googleusercontent.com/_W7vzKfSkTVE/TT6ap_ePbwI/AAAAAAAAEfs/p8V1lXAX4zM/s512/screen_shot-12193.png" alt="" />

<span style="color: #888888;">打包后图片丢失，不过问题不大</span>
### 通过Instapaper
我自己并不会把Google Reader中所有文章都投递到Kindle上，因为在GR里面需要静下心来慢慢读的文章没有那么多。我会在Google Reader里面将需要精读的文章保存到instapaper（用vimperator只需一键），然后在instapapar里下载mobi文件到kindle上阅读，算是做一遍筛选吧，这样一周需要在Kindle上读的也没有多少篇。另外，这样内容也不仅仅限制在Google Reader的文章里，只要网页都可以。Instapaper处理之后图片都还在（其实可以做一个每周Kindle精选什么的）。

当然，instapaper也可以投递到@free.kindle.com这个邮箱，下载到电脑上阅读即可。设置地址在http://www.instapaper.com/user/kindle

<img class="picasa" src="https://lh4.googleusercontent.com/_W7vzKfSkTVE/TT6ake7gJjI/AAAAAAAAEfk/1kAKwIbc6r4/s512/screen_shot-12192.png" alt="" />

<span style="color: #888888;">其实instapaper效果最好</span>

总结：

DXG用户我还是推荐instapaper，对于K3的用户来说，似乎后一个更好用。

还有一个 @zhufengme 弄的kindle.im，直接推送内容，有兴趣的读者也可以去看看。
