---
title: "VirtualBox 配置双网卡并固定 IP"
date : '2020-11-20T19:32:25-05:00'
description: "详细讲解如何在 VirtualBox 中配置双网卡（NAT + Host-Only），并为虚拟机设置静态 IP"
draft : false
featured_image : "/images/programming/VirtualBox 配置双网卡并固定IP.webp"
categories: programming
tags: [linux, network,virtualbox]
---

<br/>

# 操作概述

## 虚拟机环境

- CentOS7

<br/>

<br/>

## 开启双网卡

<center>

![](https://github.com/ErnestoIgnacio/picx-images-hosting/raw/master/ErnestoIgnacioBlog/image.1ap9wfz19z.webp)

</center>



<br/>

<img src='https://github.com/ErnestoIgnacio/picx-images-hosting/raw/master/ErnestoIgnacioBlog/image.8adjecawek.webp' width='100%' />

<br/>

<br/>

## 查看虚拟机的服务器地址

- 安装虚拟机后需要重启一次才可以看到

<img src='https://github.com/ErnestoIgnacio/picx-images-hosting/raw/master/ErnestoIgnacioBlog/image.361up2cmok.webp' width='100%' />

<br/>

<img src='https://github.com/ErnestoIgnacio/picx-images-hosting/raw/master/ErnestoIgnacioBlog/image.73u85qnuil.webp' width='100%' />

<br/>

<br/>

## 设置固定IP

```shell
vim /etc/sysconfig/network-scripts/ifcfg-enp0s3
```

```shell
TYPE=Ethernet
PROXY_METHOD=none
BROWSER_ONLY=no
BOOTPROTO=static # 设置静态IP
DEFROUTE=yes
IPV4_FAILURE_FATAL=no
IPV6INIT=yes
IPV6_AUTOCONF=yes
IPV6_DEFROUTE=yes
IPV6_FAILURE_FATAL=no
IPV6_ADDR_GEN_MODE=stable-privacy
NAME=enp0s3
UUID=9f9e8d3b-a7ad-450a-a6c8-9973fd57ebb7
DEVICE=enp0s3
ONBOOT=yes # 设置yes
IPADDR=192.168.56.110 # 设置固定的ip地址
```

```shell
# 重启网络，使得配置生效
systemctl restart network
```

<br/>

<br/>

<br/>
