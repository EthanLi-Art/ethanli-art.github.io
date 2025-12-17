---
title: 'Docker Learning Notes'
date: '2025-12-13T19:53:44-05:00'
description: "Docker Learning Notes"
featured_image: https://github.com/EthanLi-Art/picx-images-hosting/raw/master/site/image.6pnytrn10d.webp
categories: cloud-native
tags: [Docker,container,cloud-native]
comment: false
hidden: false
draft : true
---

<br/>

# 容器技术概述

## 容器发展简史

- 90年代的PC
- 00年代的虚拟化
- 10年代的cloud
- 11年代的container

<br/>

<br/>

## 什么是 container

- **容器是一种快速的打包技术**
- **容器的特点**：
  - 标准化
  - 轻量级
  - 易移植

<br/>

<br/>

## 为什么容器技术会出现？

- Linux Container容器技术的诞生于2008年（Docker诞生于2013年），解决了IT世界里“集装箱运输”的问题。Linux Container（简称LXC）它是一种内核轻量级的操作系统层虚拟化技术。Linux Container主要由Namespace和Cgroups 两大机制来保证实现
  - Namespace主要用于资源的隔离（诞生于2002年）
  - Cgroups(Control Groups)就负责资源管理控制作用，比如进程组使用CPU/MEM的限制，进程组的优先级控制，进程组的挂起和恢复等等

<br/>

<br/>

## 容器的标准化

> docker != container

- 在2015年，由Google，Docker、红帽等厂商联合发起了OCI（Open Container Initiative）组织，致力于容器技术的标准化

### runtime spec（容器运行时标准）

- 简单来讲就是规定了容器的基本操作规范，比如如何下载镜像，创建容器，启动容器等

<br/>

### image spec（容器镜像标准）

- 主要定义镜像的基本格式

<br/>

<br/>

## 容器是关乎“速度”

- 容器会加速你的软件开发
- 容器会加速你的程序编译和构建
- 容器会加速你的测试
- 容器会加速你的部署
- 容器会加速你的更新
- 容器会加速你的故障恢复

<br/>

<br/>

<br/>

# Docker 快速上手

## 安装 Docker

```shell
# linux 安装docker

curl -fsSL get.docker.com -o get-docker.sh

chmod +x get-docker.sh

sh get-docker.sh
```















<br/>

<br/>

<br/>

# 第X章











<br/>

<br/>

<br/>

# Reference





<br/>

<br/>

<br/>

# remark

> 1.

<img src='' width='70%' />
