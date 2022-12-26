---
layout: page
title: 个人博客添加第三方livere评论功能
date: 2022-12-26
excerpt_separator: "<!--more-->"
categories:
     - 网站设计
---

一千个读者就有一千个哈雷姆特，让读者在你的留言板上面留下足迹吧

<!--more-->
### 常见的第三方评论系统
* 畅言
* 多说
* 友言
* 网易云跟帖
* disqus
* gitment
### 具体操作
# 第一步：申请账号[<font>livere</font>]( https://www.livere.com/)
不需要网页域名备案，填入自己的网页域名就可以啦，顺便可以把livere账号和自己的社交账号绑定
# 第二步：管理后台
* 登录之后点击右上角的管理界面，进入后台，第一次登录会出现一个弹窗，点击实行
![](/assets/images/web design/houtai.png)
* 弹出窗口，填入信息提交就行了，其中的名称其实就是个备注，后期也可以修改的，网址别忘了带http的头
* 弹出来一段代码，选择**一般网址**就可以了（如果没弹出来也不要紧，重新登录到后台，选择**代码管理**），复制代码
![](/assets/images/web design/yibanwangzhi.png)
* 将打开GitHub项目中的**post.html**
* 将代码找到合适位置粘贴一下，一般实在文章的下面，备案信息的上面
* 到现在就结束了，不过还可以再多改一些设置，打开**livere管理界面**可以添加评论提醒，我感觉这个功能也相当实用，有新评论的的时候可以有邮件提醒
![](/assets/images/web design/tixing.png)
这样就完成了评论功能的设置，看看大家会给你评论些什么吧