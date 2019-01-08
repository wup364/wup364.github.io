---
layout: post
title:  "windows RabbitMQ service install 失败"
date:   2018-05-20 15:14:50 +0888
categories: Exception
tag: RabbitMQ
---

* content
{:toc}


X:XX/XX/X: Warning, could not set correct service description (comment)  
Error: 句柄无效(有时乱码)

解决方式:  
	1、卸载erlang  
	2、去注册表里HKLM/SOFTWARE/Ericsson/Erlang/ErlSrv下的项清掉,HKLM就是HKEY_LOCAL_MACHINE的简称  
	3、重新已管理员身份安装erlang  
	4、重新运行  