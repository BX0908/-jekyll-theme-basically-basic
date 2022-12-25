---
layout: page
title: 在Jekyll搭建经常出现各种404报错？
date: 2022-12-24
excerpt_separator: "<!--more-->"
categories:
     - 网站设计
---

我自己在搭建Jekyll过程中遇到很多404情况

<!--more-->
### _config.yml修改后404报错？
#### url与baseurl出现错误
* 可能是":"后面忘记空格
* 输入的baseurl与url格式错误
* 引号应该在英文输入法的情况下输入
![](assets/images/web design/url.png)
* [<font>yml除错工具</font>]( http://www.yamllint.com/)可以根据自己工具对yml的语言进行排错误
![](assets/images/web design/yml chucuo.png)

## Gitee Pages部署失败出现404？
* 检查管理-基本设置中仓库名称、路径、主页是否名称一致
![](assets/images/web design/warehouse.png)

### Jekyll导航栏404报错？
首先我们需要知道关于Jekyll的目录
![](assets/images/web design/jekyll mulu.png)

* 每个分类文档的头部书写规范
![](assets/images/web design/分类.md.png)
![](assets/images/web design/分类文档头部.png)

* 在文件夹_data/theme.yml中navigation_page:中添加-分类名称.md导航
![](assets/images/web design/navigation_pages.png)

### 文章上传之后没有正常显示出来？
* 上传文章时，头部要规范书写
![](assets/images/web design/对于导航.png)
* 文件命名要按照"年-月-日-##"来规范命名

#### tips：由于Gitee Pages的反应可能不够快，在重新page一遍之后，如果网站没有变化
* ①：可以用删除浏览器的历史记录的方法
* ②；重新启动一次电脑

