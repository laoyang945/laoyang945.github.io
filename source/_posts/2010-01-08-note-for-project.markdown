---
layout: post
title: '项目记录笔记软件选择'
date: 2010-1-8
wordpress-id: note-for-project
comments: true
---
昨天和实验室工程师讨论项目之后，发现自己虽然每次开会或者讨论的时候自己有做笔记，但是总没有在之后项目进行过程中把这些笔记和心得及时整理出来，因此有时候明明已经解决的问题，但是在下一步的工作中还是忘了解决。所以觉得有必要在项目过程中随时保持一个有关项目的电子文档，里面需要列出项目相关的各种文档（设计，参考，讨论纪要等）还有记录我的一些想法。

因此呢，考虑找一种笔记软件，要求如下：
<ul>
	<li>树状列表/大纲视图，可以做项目的分解</li>
	<li>能够导出/本身就是文本格式，方便以后接手的新人阅读</li>
	<li>方便插入超链接</li>
	<li>轻量级</li>
	<li>最好能支持LaTex语法</li>
</ul>
于是去了<a href="http://xbeta.info" target="_blank">善用佳软</a>的页面，找到了好几篇讲相关内容的，包括<a href="http://xbeta.info/minipad2.htm">minipad2: 性能优,功能多,体积小的笔记软件 (1)</a>，<a href="http://xbeta.info/5-treenote.htm">超级小巧的5款免费树状笔记软件 (现推荐minipad2)</a>，<a href="http://xbeta.info/tobu.htm">Tobu: 海量文本信息管理软件</a>，<a href="http://xbeta.info/vimwiki.htm">Pkm工具：Vimwiki</a>，<a href="http://xbeta.info/outliners.htm">outliner:大纲式资料管理软件对比</a>，<a href="http://xbeta.info/cintanotes.htm">CintaNotes:替代EverNote的轻量级笔记软件</a>，<a href="http://xbeta.info/pkm2.htm">PKM2：优秀的个人知识管理工具</a>。然后用半个小时下载了CintaNotes,minipad2,Tobu,pkm2,theguide,treepad,LyX,Wikidpad,gvim+vimwiki这几款软件，用两个小时左右比较了一下各自的功能和我的需求，颓然的发现好像都没有合适的……

可以做一个表格，大致说一下我的发现：
<table border="1" cellspacing="0" cellpadding="2" width="539">
<tbody>
<tr>
<td width="200" valign="top"><strong>软件</strong></td>
<td width="337" valign="top"><strong>不合适之处</strong></td>
</tr>
<tr>
<td width="200" valign="top">CintaNotes</td>
<td width="337" valign="top">不能加链接</td>
</tr>
<tr>
<td width="200" valign="top">minipad2</td>
<td width="337" valign="top">同上</td>
</tr>
<tr>
<td width="200" valign="top">Tobu</td>
<td width="337" valign="top">一个item只能加一个超链接</td>
</tr>
<tr>
<td width="200" valign="top">pkm2</td>
<td width="337" valign="top">插入链接很麻烦，不能直接拖文件</td>
</tr>
<tr>
<td width="200" valign="top">theguide</td>
<td width="337" valign="top">链接很完美，但是只能保存自己的gde格式</td>
</tr>
<tr>
<td width="200" valign="top">treepad(lite)</td>
<td width="337" valign="top">链接有点傻，不能用鼠标直接点</td>
</tr>
<tr>
<td width="200" valign="top">Lyx</td>
<td width="337" valign="top">安装未成功，一直报缺文件需下载</td>
</tr>
<tr>
<td width="200" valign="top">Wikidpad1.9rc2</td>
<td width="337" valign="top">基本满足要求，可以导出为html</td>
</tr>
<tr>
<td width="200" valign="top">gvim+vimwiki</td>
<td width="337" valign="top">插入链接不方便（<a href="http://www.gtustudy.com" target="_blank">yibie</a>的那篇教程真是够不详细的）</td>
</tr>
</tbody>
</table>
悲剧的是，“选-用-想“之后，发现其实MS Word其实才是最适合的。
<ul>
	<li>大纲视图</li>
	<li>基本上所有电脑都能读，也能导出为html（切记要导出为html，不是htm，否则代码很冗余）</li>
	<li>加相对路径的超链接很方便</li>
	<li>不算轻量级，但是也没那么重，自己比较熟悉</li>
	<li>mathtype也可以做公式</li>
</ul>
其实用Onenote也是可以的，不过我因为是两台电脑，同步还是挺成问题的，而且网摘一般都在scrapbook里面，不想再换地方了。

<a href="http://xbeta.info" target="_blank">善用佳软</a>上面有一个留言说得很好：
<blockquote>大多数人选笔记软件的时间都比记笔记的时间长</blockquote>
