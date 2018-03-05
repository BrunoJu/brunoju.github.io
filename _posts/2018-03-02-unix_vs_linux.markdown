---
layout:     post
title:      "Unix and Linux"
date:       2018-03-02 17:00:00
author:     "BrunoJu"
header-img: "img/post/unix_vs_linux.jpg"
comment:    true
tags:
    - kernel
---
# 历史
```
1973年， 脱胎于Multics系统的Unix用C语言进行了一次重写，为其强大的移植性铺平了道路。
1977年，加州大学伯克利分校推出基于Unix的变体BSD，并提供了源码（macOS就是BSD版本的后裔)
1991年，Linus基于Intel 80386微处理器开发了一套全新的系统,Linux由此诞生
```

## Unix强大的原因

- Unix的代码简洁
- 所有文件都被当文件对待（除了socket)
- 内核与相关系统工具是C写成，因此移植性强
- Unix的进程创建非常迅速 (fork函数)
- 有一套非常简单又稳定的进程间通信元语



## Linux优于Unix的特点
- 支持动态加载内核模块，尽管Linux的内核也是单内核
- 支持对称多处理机制SMP
- 内核可以抢占，Linux内核具有允许在内核执行的任务优先执行的能力
- 内核不分进程和线程，所有的进程都一样——只不过是其中的一些共享资源而已
- 提供具有设备类的面向对象的设备模型、热插拔事件，以及用户的设备文件系统sysfs
- 遵守Unix API（Posix)，但忽略了一些被认为设计的很拙劣的Unix特性，像STREAMS
- 体现了自由的精髓，简洁的设计，可靠地实现


## 单内核的Linux同时具有微内核特性
- 模块化设计
- 抢占式内核
- 支持内核线程
- 支持动态加载内核模块
