---
title: "对接tg"
description: "仅分享新版傻妞使用记录，如有不对请指正"
keywords: "傻妞,TG"

date: 2022-12-08T21:31:54+08:00
lastmod: 2022-12-08T21:35:36+08:00

categories:
  - 傻妞专题
tags:
  - 傻妞
  - TG

url: sillygirl/TG.html
toc: true
---

> 此记录基于2022年12月2号的版本，在此之前或之后的版本仅供参考。以下任何命令如果没有说明则表示是在交互界面执行。
首先你需要正确安装傻妞，参考[从得到到抛弃](getToThrow.html)
其次你需要完成 [创建TG机器人](creatTgBot.html)
然后你的傻妞需要能科学上网

## 对接TG机器人

### 安装TGbot插件

在插件市场找到 **Telegram Bot，点击安装**

![image.png](TG/image.png)

### 设置机器人信息

```Shell
set tg token <token>
```

此处填写从[创建TG机器人](creatTgBot.html)获得的机器人token

> 请不要一个机器人对接多个程序！！！

![image.png](TG/image1.png)

### 设置管理员

```Shell
set tg masters <你的ID>
```

不知道自己ID的给机器人发送 `myuid`

完成。就是这么简单。

## 对接人型bot

不知道人型bot的先去了解一下，官方频道

[PagerMaid-Modify Update](https://t.me/PagerMaid_Modify)

即将分离该功能，暂不更新。