---
title: '《Python3.8 系统入门 + 进阶》Course Notes'
date: '2025-11-23T16:39:14-05:00'
description: "《Python3.8系统入门+进阶 (程序员必备第二语言)》课程的学习笔记，涵盖基础语法、核心模块与项目实战"
featured_image: "https://github.com/EthanLi-Art/picx-images-hosting/raw/master/site/image.6wr5wfiks2.webp"
categories: "Programming"
tags: ["Python", "Course Notes", "Programming"]
comment: false
hidden: false
draft : false
---

<br/>

# 概述







<br/>

<br/>

<br/>

# 第2章 Python环境安装

## 如何有效提问

- 略

<br/>

<br/>

## Python学习建议

- 如何学习这门课

  - 认真看视频
  - 跟着视频写代码
  - 课后思考题尽量完成，即使完成不了也需要也要跟着思考

- 配套书籍

  - 跟着视频学习就不需要其它基础教程了
  - 唯一推荐《流程的Python》，作为高级内容的补充

- 有必要做习题吗？

  - 不推荐
  - 编程的目的是为了解决问题

- 后续学习方向

  - web开发（使用python做web开发更适合个人开发者）
    - 数据库、选择一个web框架（Django，Flask）
  - 数据分析
    - 误区：看重工具（库、框架）的学习
    - 重点：数学模型
  - AI
    - Python只是辅助，重点学习AI相关的知识
  - 工作效率，自动化处理
    - 搜索

  <br/>

  <br/>

## 版本选择

- 建议安装Python 3.8
- 多版本安装：使用虚拟环境

<br/>

<br/>

<br/>

# 第3章 理解什么是写代码与Python的基本类型

## 前言

- 什么是代码：代码是现实世界事物在计算机世界中的映射
- 什么是写代码：将现实世界中的事务用计算机语言来描述

<br/>

<br/>

## 基本数据类型

- Number
  - 整数：int（其它语言中对整数可能还有细分，但在Python中只有int）
  - （小数）浮点数：float [其它编程语言中有双精度（double）和单精度（float）之分，但Python中没有这种区分，默认float直接对应其它编程语言中的双精度]

```python
# Python中两个整数（或者任何数）相除会得到float类型
>>> type(4/2)
<class 'float'>

# 如果想让结果得到整数类型，需使用 // ，// 表示整除
>>> type(4//2)
<class 'int'>

>>> type(5//2)
<class 'int'>
```



- 进制的表示与转换

```python
# 二进制
0b1010

# 八进制
0o10

# 十六进制
0x1F


# 任意进制转二进制
bin(xxx)

# 转十进制
int(xxx)

# 转16进制
hex(xxx)

# 转八进制
oct(xxx)
```



- bool（布尔）类型
  - True
  - False

```python
# False
bool(0)

# 所有非0是True
```

- 其它类型可以向bool类型转换
- 一般情况：
  - 非空会被转换成True
  - 空值会被转换成False



- complex（复数）类型
  - 36j
- str 字符串
  - 字符串的表示：单引号，双引号，三引号
  - 转移字符
  - 字符串的运算















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
