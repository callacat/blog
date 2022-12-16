---
title: "尝试编写一个简单的脚本并发布"
description: ""
keywords: "傻妞"

date: 2022-12-13 17:22:11+08:00
lastmod: +08:00

categories:
  - 傻妞专题
tags:
  - 傻妞

url: 
toc: true
---

> 仅做学习，大佬勿喷

## 编写脚本

在插件市场下载插件开发长插件，可以看到猫把大部分内置命令都写出来了，复制粘贴搞起来

首先，我的目的是编写一个获取短网址的插件，使用api地址`https://xiaoapi.cn/API/dwz.php?url=`来进行短网址生成，然后返回

先把插件信息写好

```Shell
/**
 * @author Dswang
 * @origin Dswang
 * @create_at
 * @description suol.cc短网址生成
 * @version v1.0
 * @title 短网址生成
 * @rule raw ^dwz (.*)$
 * @priority 100
 * @public false
 * 脚本图标。
 * @icon https://xiaoapi.cn/favicon.ico
 */
 ```

 以上信息对于短网址生成来说足够了，脚本图标直接使用了api提供网站的图标。如果想在未来发布改脚本，则需要将`@public`设为true

 然后开始编写剩下的内容

 ```Shell
//首先创建一个sender对象
const s = sender
//获取用户输入的域名
const url = s.param(1)
//请求网络并获取返回内容


 ```
