---
title: "安装nark"
description: "仅分享新版傻妞使用记录，如有不对请指正"
keywords: "傻妞,nark,Docker"

date: 2022-12-08T16:40:59+08:00
lastmod: 2022-12-08T21:01:07+08:00

categories:
  - 傻妞专题
tags:
  - 傻妞
  - nark
  - Docker

url: sillygirl/install-nark.html
toc: true
---
> 首先你得有授权，没有请忽略
其次请先 [安装Docker](install-Docker.html)

## 手动安装

首先新建一个文件夹，进入文件夹后执行

```Shell
docker run -dit \
--name nark \
-p 5704:80 \
--restart=always \
-v "$(pwd)"/Config:/app/Config \
-v "$(pwd)"/logfile:/app/logfile \
nolanhzy/nark:latest
```

将授权文件放入 `"$(pwd)"/Config`，重启nark

```Shell
docker restart nark
```

### 更新

```Shell
docker run --rm -v /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower -c --run-once nark
```

或者 [快速更新容器](install-docker/install-portainer.html#快速更新容器)

## 一键脚本

找不到了，自己去群里找吧