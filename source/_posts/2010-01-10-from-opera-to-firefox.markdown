---
layout: post
title: '从Opera转到Firefox'
date: 2010-1-10
wordpress-id: from-opera-to-firefox
comments: true
---
大概从5年还是6年前，我就开始用Opera作为我的主浏览器。一直很喜欢，还在我的博客里面写了不少文章来介绍Opera，比如<a href="http://laoyang.info/blog/?p=1762" target="_blank">[日常软件使用技巧]12.我最喜爱的浏览器--Opera</a>以及<a href="http://laoyang.info/blog/?p=35297" target="_blank">关于Opera的一些想法</a>。说实话我觉得Opera是一个不需要太多配置就可以用好的浏览器。但是有几个原因迫使我在去年的冬天从Opera转到了Firefox：
<ul>
	<li>Autoproxy，用处打地道。Opera只能自己写pac文件，太麻烦了。Autoproxy的列表可以订阅更新，这就很好。而且Opera还不支持socks代理</li>
	<li>感觉Opera和Google的关系不怎么好，用Gmail和Google Reader的时候明显的感觉载入会慢。时不时的还会出现排版错乱。而且Opera的user script<span style="text-decoration: line-through;">只能针对一个站点</span>不能调整在一个站点中的使用范围，这就很郁闷了。我还得把各个脚本集合起来，然后根据url的不同来区别对待。</li>
	<li>Opera上淘宝很奇怪的会有时候没图</li>
	<li>Opera原生不支持带格式复制，这很郁闷。（Firefox原生不支持纯文本复制，这也很郁闷）</li>
</ul>
其实后面两点还好，主要是第一点驱使我使用Firefox，并且我感觉Opera的用户还是太少，对站点来说估计不会考虑做专门的测试。

现在用了将近两个月的Firefox，感觉还好。需要配置一下，不过也不算复杂，实现Opera的自带功能需要的Firefox对应扩展如下：
<table border="1" cellspacing="0" cellpadding="2" width="490">
<tbody>
<tr>
<td width="222" valign="top"><strong>Opera自带功能</strong></td>
<td width="266" valign="top"><strong>Firefox所需对应扩展</strong></td>
</tr>
<tr>
<td width="222" valign="top">同步书签</td>
<td width="266" valign="top">Weave/XMarks，后者须翻墙</td>
</tr>
<tr>
<td width="222" valign="top">笔记(无格式文本)+同步笔记</td>
<td width="266" valign="top">zotero/scrapbook+dropbox</td>
</tr>
<tr>
<td width="222" valign="top">粘贴并转到</td>
<td width="266" valign="top">paste and go</td>
</tr>
<tr>
<td width="222" valign="top">隐藏菜单栏</td>
<td width="266" valign="top">Personal Menu</td>
</tr>
<tr>
<td width="222" valign="top">跳转至URL</td>
<td width="266" valign="top">Take me to url</td>
</tr>
<tr>
<td width="222" valign="top">鼠标手势</td>
<td width="266" valign="top">All in one gestures</td>
</tr>
<tr>
<td width="222" valign="top">快捷键设定</td>
<td width="266" valign="top">keyconfig</td>
</tr>
<tr>
<td width="222" valign="top">广告过滤(A.shun说还有Adblock+很好用)</td>
<td width="266" valign="top">Adblock Plus（功能更强）</td>
</tr>
</tbody>
</table>
由于Firefox用户较多，所以淘宝开发了淘宝旺旺的协议扩展，这样就能从Firefox里面启动旺旺了，好像Opera经过什么设置也是可以的。另外FlashGot和一个能看youtube视频的油猴脚本也很好用。

使用的扩展大多数已经整理在<a href="https://addons.mozilla.org/zh-CN/firefox/collection/laoyang945" target="_blank">我的扩展列表收藏集</a>里面，需要参考的可以去看看

最后Firefox被我折腾成了Opera的顺心功能+Chrome的外观的混合体。收藏栏的效果，只需要把标题去掉只保留图标就行，可以安装一个IdentFavIcon来重载网站图标

<a href="http://laoyang.info/blog/wp-content/uploads/2010/01/image.png"><img style="display: inline; border: 0px;" title="image" src="http://laoyang.info/blog/wp-content/uploads/2010/01/image_thumb.png" border="0" alt="image" width="484" height="350" /></a>
