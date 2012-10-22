---
layout: post
title: '时间管理软件Chandler使用介绍[1]'
date: 2008-11-26
wordpress-id: chandler-get-started
comments: true
---
    Chandler是一个符合GTD思想的时间管理软件，它不但集成了日程管理和任务管理，还有邮件处理功能。另外，它还可以有网络同步功能，使你在任何地方都可以使用。软件的目标是很远大的，它要做Outlook杀手。这一篇日志将教会你Chandler的基本使用

    1.下载、安装及汉化

    在<a href="http://cid-1d3a12f9809b6d8e.skydrive.live.com/self.aspx/%e8%bd%af%e4%bb%b6/Chandler1.0.2.rar" target="_blank">这里</a>可以下载已经汉化好的1.0.2版本

    如果想自己汉化的话，看看<a href="http://code.google.com/p/chandlercn/wiki/Chandler_FAQ?ts=1230771330&amp;updated=Chandler_FAQ" target="_blank">http://code.google.com/p/chandlercn/wiki/Chandler_FAQ?ts=1230771330&amp;updated=Chandler_FAQ</a>，这样能在使用中对不满意的词条进行修改

    2.基本概念(参考Chandler Get Started Guide）

    Chandler里面基本的信息单元是“条目”-item，依照条目的属性不同，分为“便条note”，“加星便条starred note”和“事件event”三类。三类间可以互相转换。可以通过邮件发送条目

    比条目高一级的是“分类”，分类和条目是多对多的关系。由于条目的属性不同，分类可以有三种视图，分别是“所有条目”“加星标的”“日程表”，其中日程表只显示有时间属性的事件。

    每一个条目有三个状态：NOW LATER DONE。正如字面的意思。当事件未开始的时候，自己会标为LATER，开始了之后自动标记为NOW

    3.界面介绍

    运行d:\Chandler\chandler.exe，就可以启动Chandler了，第一次启动会比较慢，请耐心等待。完成启动过程后，界面如下图所示：

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-210546.png"><img border="0" width="504" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-210546-thumb.png" alt="2008-11-26_210546" height="364" style="display: inline; border: 0px" title="2008-11-26_210546" /></a>

    我们从左到右的介绍一遍：

    分类栏中，有默认的四个系统分类——“Dashboard””In””Out”和“垃圾箱”，其中Dashboard我觉得对应的是GTD中收件箱的概念，Dashboard中不能使用日程表视图，你在快捷输入栏或者条目-新建中所创建的所有条目都会进入Dashboard分类里面。或许可以翻译为“工作篮”。In和Out分别是对应邮件的收件箱和发件箱。
你也可以建立自己的分类，就像上图中的工作、家庭、娱乐和US节日一样，方法是在分类栏内右击后选择新分类或者工具栏中的分类-新建。

    日历就是日历啦，没什么好介绍的，可以

    在条目列表里面，可以看到当前分类里面的条目。

    在条目详情里面，可以看到当前选定条目的详情

    在视图选择里面，可以选择针对当前分类的视图类型，在快捷输入栏里面，可以快速新建一个条目。

    快捷输入栏右边的“清理”(我觉得译为整理比较好)，可以迅速帮你把条目列表中的条目按照其状态整理好。

    4.开始使用

    下面我们为了使用的方便，将默认存在的条目全部删除掉。方法是选中Dashboard后，在条目列表里按Ctrl+A，然后Del。Ooops，它会提示你“US 节日是只读的/仅供查看的”,不能删除。你可以先把其他的删除掉。然后在US节日上点右键，然后选择“退订”就可以删除了，现在你的Chandler应该是这样：

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214057.png"><img border="0" width="504" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214057-thumb.png" alt="2008-11-26_214057" height="364" style="display: inline; border: 0px" title="2008-11-26_214057" /></a>

接下来，我们在快捷输入栏（就是有创建新便条）的那一栏输入一个事项，比如“买《像艺术家一样思考》”，回车后应该是像下图一样：

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214421.png"><img border="0" width="504" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214421-thumb.png" alt="2008-11-26_214421" height="348" style="display: inline; border: 0px" title="2008-11-26_214421" /></a>

在右边的详情栏里面，可以进行的操作有：

1.写一些备注：比如图中的“听说这是一本不错的书”
2.加星标，点<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214640.png"><img border="0" width="29" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214640-thumb.png" alt="2008-11-26_214640" height="30" style="display: inline; border: 0px" title="2008-11-26_214640" /></a> 可以加星标
3.发送，点<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214647.png"><img border="0" width="33" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214647-thumb.png" alt="2008-11-26_214647" height="28" style="display: inline; border: 0px" title="2008-11-26_214647" /></a> 可以用电子邮件发送当前条目（电子邮件账户配置在下一篇文章）
4.安排时间，点<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214700.png"><img border="0" width="26" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214700-thumb.png" alt="2008-11-26_214700" height="33" style="display: inline; border: 0px" title="2008-11-26_214700" /></a>可以对这个条目安排时间
5.转换状态，如图的状态是NOW，通过点击NOW可以在三种状态中转换。

下面我点 <a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-2147001.png"><img border="0" width="26" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-214700-thumb1.png" alt="2008-11-26_214700" height="33" style="display: inline; border: 0px" title="2008-11-26_214700" /></a>来为买书安排时间

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-215208.png"><img border="0" width="279" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-215208-thumb.png" alt="2008-11-26_215208" height="455" style="display: inline; border: 0px" title="2008-11-26_215208" /></a>

到时候Chandler就会在11-28的11：45跳出来提醒我了~

下面我们新建一个分类，叫做Amazon，在工具栏的“分类”项下可以对分类做设置，其中，不在Dashboard里面显示的意思是分类及其下包括的条目不在Dashboard里面显示。我们把颜色设置一下：

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-215538.png"><img border="0" width="271" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-215538-thumb.png" alt="2008-11-26_215538" height="314" style="display: inline; border: 0px" title="2008-11-26_215538" /></a>

    然后我们可以把刚才新建的那个“买《》”的条目拖到Amazon的分类里面去，然后选择日程表视图，可以看到，我们刚才的那个条目已经出现在日程表里面了。同时，日程表是覆盖显示的，也就是说当你选择多个分类时，各分类中的条目可以同时显示在日程表里面。

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-215934.png"><img border="0" width="504" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-215934-thumb.png" alt="2008-11-26_215934" height="321" style="display: inline; border: 0px" title="2008-11-26_215934" /></a>

  <a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-220539.png"><img border="0" width="244" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20081126-220539-thumb.png" alt="2008-11-26_220539" height="208" style="display: inline; border: 0px" title="2008-11-26_220539" /></a> 分别是娱乐和Amazon中的条目=========================以上是内容===========================

   在汉化的过程中，难免有错误，希望大家在使用的时候指正~

    欢迎到<a href="http://code.google.com/p/chandlercn/">http://code.google.com/p/chandlercn/</a>提交问题
