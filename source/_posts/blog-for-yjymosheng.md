---
title: blog_for_yjymosheng  殷金钰
date: 2024-11-09 22:34:33
tags:
---

# 阶段一总结

## 初次认真学习rust每一个点 ##

通过某些渠道，第一次了解到操作系统训练营，以前我也有用rust写过一些内容，但严格来说这是我的第一次正式学习rust。学习了很多的内容，了解到了
闭包，函数式编程，拓展了我的知识面，我第一次见到结构如此清晰的语言。

## 所有权的理解 ##

众所周知，rust很贪。所有权是其中的灵魂。我认为，其本质就是“作茧自缚”，减少了许多东西，又为方便开发与调试添加了许多东西。这些设计减少了许
多的错误。所以简单的把所有权当作单线程的脑子就行，不要给它过多的行为。

## 错误处理中的Option Result ##


- Option 用于表达可能存在或者不存在的值，它有两种可能的状态：Some(值) 和 None。当你不确定一个值是否存在时，可以使用 Option 来处理这种情
况。

- Result 则用于表达可能的操作成功或失败的结果，它有两种可能的状态：Ok(值) 和 Err(错误)。当你需要处理可能出现错误的情况时，可以使用 Result 来处理这种情况。

## 令人耳目一新的枚举类型 match ##

在 Rust 中，枚举类型是一种非常强大的数据结构，它可以用来表达一组相关的值。而使用 match 关键字可以让我们更加灵活地处理枚举类型的值，使得
代码更加清晰易懂。

match 表达式可以用来匹配枚举类型的不同变体，并根据不同的情况执行相应的代码逻辑。这种模式匹配的方式让代码的逻辑结构清晰明了，同时也增强了
代码的可读性和可维护性。

## 我的收获 ##

通过学习 Rust，我收获了很多。不仅仅是语言本身的特性和语法，更重要的是 Rust 给我带来的编程思维方式的转变。在学习 Rust 的过程中，我更加注
重代码的安全性和可靠性，学会了如何利用 Rust 的各种特性来编写更加健壮的程序。

另外，通过与社区的交流和分享，我还了解到了很多其他开发者的经验和见解，这也让我受益匪浅。总的来说，学习 Rust 是一次非常有意义的经历，我相
信在将来的工作和项目中，我会继续运用 Rust 的知识和思想，为我的编程生涯注入新的活力和动力。



# 阶段二总结

在rcore的实验课程中，最让我印象深刻的就是虚拟地址部分，由于之前接触的操作系统全部都是nommu类型，直接访问物理地址的概念非常不容易被打破，并且ch4也是一个门槛，需要非常深入的理解rcore的整体代码框架，对虚拟地址的映射，软硬件协同操作，多级页表，地址空间的概念理解了很久，在不断查找资料，不断理解的情况下，才对虚拟地址的概念有了很浅显的理解，把任务完成。

在完成任务的过程中，其实rcore的整体框架非常完善，作业的部分也就是一些扩展功能，整体还是对rcore的实现的理解，在完成任务时，也是对已有实现进行模仿，理解整体框架，之后调用已有函数或自己根据数据结构实现函数，实现功能。

以及最后两个lab难度上升有点大，并且文章 中是对功能的描述居多(很多对于实验有用的点会被淹没在其中)虽然在边做lab边反复查看资料时可以发现，但是对于没有接触过的同学可能很多api看过就没印象了，在后续做lab中也找不到，所以可以适当增加一下强调或者提示，来减少难度增加坡度。