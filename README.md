# 《Windows 内核安全编程技术实践》

<div align=center>
<img width="150" src="https://user-images.githubusercontent.com/52789403/201465673-01dd7d47-7092-4523-b828-8af16030b979.png" />
</div>

<br>

**作者：** 王瑞<br>
**页数：** 420页<br>
**开本：** 16开<br>
**装帧：** 平装<br>
**所属分类：** 软件信息安全<br>
**兼容系统：** Windows 10 Build 18362.19h1
**作者邮箱：** me@lyshark.com<br>
**作者博客：** https://www.lyshark.com<br>

## 封面设计

![image](https://user-images.githubusercontent.com/52789403/202657410-d5259dfb-8161-4579-bb3b-5c775b9deed1.png)

<br>

## 概述

《Windows 内核安全编程技术实践》 是2023年申请登记的内核安全系列图书作品，作者是王瑞。本书内容详实、深入浅出、案例丰富，是Windows内核开发工程师的参考资料，也可供信息安全相关专业的在校学生和入门者学习参考。本书是近年来少见的关于公布Windows ARK反内核工具实现细节的相关图书。

## 内容简介

这是一本 Windows 内核安全编程系列丛书，由作者多年技术积累编写而成，该书由浅入深、循序渐进地介绍了 Windows 内核程序的开发方法与调试技巧。书如其名探索 Anti Rootkit 反内核工具核心原理与技术实现细节，本书最大的特色在于每一节的例子都是经过精挑细选的，具有很强的针对性。不同于市面上的多数 内核开发 系列丛书，本书是以内核安全角度为切入点，以实战角度出发，力求让读者通过亲自动手实验，掌握各类 Windows 内核安全编程的相关技巧，学到尽可能多的 Windows 底层知识。 本书适用于中、高级系统安全工程师，同时也可用做高校计算机专业操作系统开发实验课的补充教材。

## 关于作者

王瑞，LyShark 门户创始人，毕业于中国海洋大学（计算机科学与技术）专业，曾就职于中国联通（北京），二进制安全技术专家，持有红帽认证RHCE工程师，华为认证HCIP网络安全高级工程师，Oracle甲骨文认证数据库专家。自幼便对计算机产生了浓厚兴趣，自学二进制安全方向十余年，常在互联网博客平台分享安全技术研究经验及成果，对网络安全，安全运维，渗透测试，安全开发，软件逆向分析，计算机反病毒，等技术都具有浓厚的兴趣。

作者曾荣获51CTO博客-专家博主，华为云-云享专家，阿里云-专家博主，开源中国-推荐博主，CSDN博客-全栈领域优质创作者，CSDN博客-2022年度博客新星Top5，CSDN博客-博客专家认证，InfoQ中国签约作者，博客园-排200名，腾讯云-2022年度优秀作者。

自幼热爱计算机技术，尤其喜爱二进制安全方向，并长期致力于信息安全技术研究，自学钻研计算机技术十余年，期间没有任何人给予过任何帮助，遇到问题只能自己想办法，人最困难的时候并不是在学校求学的时光，而是在出现问题时，回头却发现身后空无一人，LyShark深知初学者的困境，并能够感同身受，发布本书只是为了无私帮助更多人，所谓前人栽树后人乘凉，知识需要积累与总结，希望你也能够将所学所想，继续传递下去。

## 撰写初衷

某一天，笔者想要实现一款`ARK反内核`工具，在找资料时发现市面上多数ARK工具都经过了`VMP`高强度`加密`，内核代码`尤为宝贵`这一点可以被`理解`，多数有源码的项目也都是`过时的`无法正常使用，故想要将ARK反内核工具功能在最新版本的`Windows 10 x64`系统上面实现，既可以`整理归纳`自己的知识体系，也可以`帮助更多`底层爱好者`学习`内核开发技术，让更多安全爱好者从中受益。

## 法律警告

本书内容首发于`博客园`，根据`《中华人民共和国著作权法》`相关规定本人享有`著作权`，本书的发放`仅用于`技术交流学习，本书内容`免费`，禁止第三方倒卖，如果您在第三方购买到本书请与作者联系，作者`(LyShark)`将追究倒卖者法律责任，纯净的技术交流需要你我共同来维护，感谢您阅读并支持作者的创作。

## 书籍目录

 - 第一章：环境配置篇
   - 1.1 WDK8.1 驱动开发环境配置
   - 1.2 WinDBG 配置内核双机调试
   - 1.3 内核测试模式过DSE签名

 - 第二章：基础知识篇
   - 2.1 内核中的链表与结构体
   - 2.2 内核中的自旋锁结构
   - 2.3 内核字符串转换方法
   - 2.4 内核字符串拷贝与比较

 - 第三章：驱动通信篇
   - 3.1 驱动与应用的简单通信
   - 3.2 应用DeviceIoContro开发模板
   - 3.3 通过SystemBuf与内核层通信
   - 3.4 通过ReadFile与内核层通信
   - 3.5 通过PIPE管道与内核层通信
   - 3.6 通过Async反向与内核通信

 - 第四章：驱动读写篇
   - 4.1 内核CR3切换读写内存
   - 4.2 内核MDL读写进程内存
   - 4.3 通过内存拷贝读写内存
   - 4.4 内核R3与R0内存映射拷贝

 - 第五章：内核SSDT解析篇
   - 5.1 内核枚举SSDT表基址
   - 5.2 内核枚举完整SSDT表
   - 5.3 枚举ShadowSSDT表基址

 - 第六章：内核进程线程篇
   - 6.1 内核中枚举进线程与模块
   - 6.2 监控进程与线程对象操作
   - 6.3 内核监控进程与线程创建
   - 6.4 内核DKOM实现进程隐藏
   - 6.5 内核中实现Dump进程转储
   - 6.6 内核遍历进程VAD结构体
   - 6.7 运用VAD隐藏R3内存思路
   - 6.8 内核摘链DKOM进程隐藏
   - 6.9 内核无痕隐藏自身分析
   - 6.10 内核强制结束进程运行

 - 第七章：内核模块篇
   - 7.1 内核判断驱动加载状态
   - 7.2 内核取ntoskrnl模块基地址
   - 7.3 内核取应用层模块基地址
   - 7.4 内核通过PEB得到进程参数
   - 7.5 断链隐藏驱动程序自身
   - 7.6 内核特征码搜索函数封装
   - 7.7 内核LDE64引擎计算汇编长度
   - 7.8 内核层InlineHook挂钩函数

 - 第八章：内核枚举篇
   - 8.1 内核枚举IoTimer定时器
   - 8.2 内核枚举DpcTimer定时器
   - 8.3 内核枚举PspCidTable句柄表
   - 8.4 内核枚举Minifilter微过滤驱动
   - 8.5 内核特征码扫描PE代码段
   - 8.6 内核枚举LoadImage映像回调
   - 8.7 内核枚举Registry注册表回调
   - 8.8 内核枚举进程与线程ObCall回调

 - 第九章：内核监控篇
   - 9.1 内核监控进程与线程回调
   - 9.2 内核注册并监控对象回调
   - 9.3 内核监视LoadImage映像回调
   - 9.4 内核运用LoadImage屏蔽驱动
   - 9.5 内核监控Register注册表回调
   - 9.6 内核监控FileObject文件回调


## 特别感谢

感谢自己对自己的不放弃，努力走自己的路，虽然无法得到别人的认可，但自已还是要认可自己！


## 许可协议

[CC BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)

[中华人民共和国著作权法](http://www.gov.cn/guoqing/2021-10/29/content_5647633.htm)

[项目地址](https://github.com/lyshark/WindowsKernelBook)
