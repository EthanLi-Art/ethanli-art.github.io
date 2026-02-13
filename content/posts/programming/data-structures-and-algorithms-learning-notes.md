---
title: 'Data Structures and Algorithms Learning Notes'
date: '2025-12-17T15:07:31-05:00'
description: "Data Structures and Algorithms Learning Notes"
featured_image: https://github.com/EthanLi-Art/picx-images-hosting/raw/master/site/image.3uvatf0uui.webp
categories: Algorithms
tags: [Algorithms, Data-Structures]
comment: true
hidden: false
draft : false
---

<br/>

# 数据结构与算法学习概述

## 算法概述

- 什么是算法：**一系列解决问题的，清晰，可执行的计算机指令**
- 算法的特点：
  - 有限性
  - 确定性：不会产生二义性
  - 可行性
  - 输入
  - 输出

<br/>

<br/>

## 学习内容概述

- 学习的主要内容
  - **十大排序算法**：插入，冒泡，选择，希尔，快速，归并，堆排序，计数排序，桶排序，基数排序
  - **查找算法**：线性查找，二分查找
  - **线性数据结构**：动态数组，链表，栈，队列，哈希表
  - **经典树结构**：二分搜索树，堆，AVL，红黑树，B 类树
  - **高级数据结构**：线段树，并查集，Trie，SQRT 分解
  - **字符串算法**：KMP，模式匹配

<br/>

- **通过学习算法与数据结构的内容，同时也深刻理解计算机科学**
  - 二分查找：
    - 如何编写正确的程序
    - 边界
    - 处理整数和浮点数的区别
  - 快速排序，归并排序，链表，树结构：
    - 递归
    - 算法的优化过程
  - 快速排序
    - 随机算法
  - 哈希表，RK 算法
    - 哈希
  - 桶排序，aqrt 分解
    - 分块
  - 线段树，sqrt 分解
    - 区间估计
  - 希尔排序
    - 没有固定写法的算法
  - KMP
    - 确定有限状态自动机
  - B 树
    - 内存和外存考量的不同
  - ...

<br/>

<br/>

<br/>

# Linear Search

- Java

```java
public class LinearSearch<E> {

    private LinearSearch() {

    }

    public static <E> int search(E [] data,E target) {
        for (int i=0;i<  data.length;i++) {
            if (data[i].equals(target)) {
                return i;
            }
        }
        return -1;
    }
    
}
```

- Go

```go
import "fmt"

/*
LinearSearch
-------------
泛型线性查找
T 必须是 comparable（支持 == 比较）
*/
func LinearSearch[T comparable](data []T, target T) int {
	for i, v := range data {
		if v == target {
			return i
		}
	}
	return -1
}

type Student struct {
	Name string
	Age  int
}
```













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
