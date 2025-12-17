---
title: "《Grokking Algorithms》Study Notes"
date: 2025-11-30T15:30:09-05:00
description: "Study notes on the book 《Grokking Algorithms》"
featured_image: "/images/programming/grokking-algorithms-notes.png"
categories: algorithm
tags:
  - algorithm
  - data-structure
  - study-notes
draft: false
---

<br/>

# 第1章 算法简介

## 二分查找

```python
# python3 实现二分查找
def binary_search(list,item):
    low = 0
    hight = len(list)-1

    while low <= hight:
        mid = (low + hight)//2
        if list[mid] == item:
            return mid
        elif list[mid] < item:
            low = mid+1
        else:
            hight = mid-1

    return None

my_list = [1, 3, 5, 7, 9]

print(binary_search(my_list,3))
print(binary_search(my_list,9))
```

<br/>

<br/>

## 大 O 表示法

- 仅知道算法需要多长时间才能运行完毕还不够，还需知道运行时间如何随列表增长而增加。这正是大O表示法的用武之地
- 大 O 表示法用于描述算法的渐进时间复杂度或空间复杂度，表示随着输入规模 n 增大，算法的运行时间（或空间使用）在数量级上的上界
- 大 O 表示法指出了最糟情况下的运行时间

<br/>

<br/>

## 算法复杂度

- 算法的速度指的并非时间，而是操作数的增速
- 谈论算法的速度时，我们说的是随着输入的增加，其运行时间将以什么样的速度增加
- 算法的运行时间用大O表示法表示
- O(log n)比O(n)快，当需要搜索的元素越多时，前者比后者快得越多
- 算法运行时间是从其增速的角度度量的

<br/>

<br/>

<br/>

# 第2章 选择排序

- 熟悉数组和；链表的增删改查的时间复杂度，以及其优势和劣势

```python
def selection_sort(arr):
    n = len(arr)
    
    for i in range(n-1):
        min_index = i
        for j in range(i+1,n):
            if arr[j] < arr[min_index]:
                min_index = j
        arr[i],arr[min_index] = arr[min_index],arr[i]
    return arr
nums = [64, 25, 12, 22, 11,90,22,23,12,4,6,3,8,99,5,5,5,4,54,5,3,543,5,43,5,43,5,543543534543]
print(selection_sort(nums))
```

<br/>

<br/>

<br/>

# 第三章 递归

- 栈只有2种操作：压入栈和弹出栈
- 递归指的是调用自己的函数
- 每个递归函数都有两个条件：基线条件和递归条件
- 栈有两种操作：压入和弹出
- 所有函数调用都进入调用栈
- 调用栈可能很长，这将占用大量的内存

<br/>

<br/>

<br/>

# 第四章 快速排序

- 快速排序使用分而治之的策略
- 使用D&C解决问题的过程包括两个步骤
  - (1) 找出基线条件，这种条件必须尽可能简单
  - (2) 不断将问题分解（或者说缩小规模），直到符合基线条件
- 











