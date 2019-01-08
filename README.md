# Peng's Blog

备忘录
====================================

博客配置
------------------------------------

项目需要配置一个文件`_config.yml`, 打开之后按照如下进行配置。

> 特别注意`baseurl`的配置。如果是`***.github.io`项目, 不修改为空''的话, 会导致JS,CSS等静态资源无法找到的错误

``` bash
name: 博客名称
email: 邮箱地址
author: 作者名
url: 个人网站
### baseurl修改为项目名, 如果项目是'***.github.io', 则设置为空''
baseurl: ""
resume_site: 个人简历网站
github: github地址
github_username: github用户名称
FB:
  comments :
    provider : duoshuo
    duoshuo:
        short_name : 多说账户
    disqus :
        short_name : Disqus账户
```

如何写文章
------------------------------------

在`Peng's Blog/_posts`目录下新建一个文件, 可以创建文件夹并在文件夹中添加文件, 方便维护。在新建文件中粘贴如下信息, 并修改以下的`titile`,`date`,`categories`,`tag`的相关信息, 添加`* content {:toc}`为目录相关信息, 在进行正文书写前需要在目录和正文之间输入至少2行空行。然后按照正常的Markdown语法书写正文。

``` bash
---
layout: post
#标题配置
title:  标题
#时间配置
date:   2016-08-27 01:08:00 +0800
#大类配置
categories: document
#小类配置
tag: 教程
---

* content
{:toc}


我是正文。我是正文。我是正文。我是正文。我是正文。我是正文。
```