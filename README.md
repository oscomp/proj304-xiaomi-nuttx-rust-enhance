# proj304-xiaomi-nuttx-rust-enhance
# 基于小米Vela平台的NuttX RTOS Rust增强

## 项目描述

### 平台介绍

**关于小米澎湃OS**：小米澎湃OS是一款以人为中心、打造「人车家全生态」的操作系统。小米澎湃OS经过 13 年探索，历时 7 年研发，参与的工程师超过5000名，进行了史无前例的系统底层重构，为未来百亿设备、百亿连接做好「万物互联的公有底座」。

2017年，小米自研的Vela OS正式发布，逐步统一IoT设备生态。2019年，小米开始并行研发纯自研通用系统Mina OS。2021年，小米开启了车机OS的研发。2022年初，小米统一MIUI、Vela、Mina、车机OS四个系统的软件架构，自此小米的操作系统底层合并完成。

小米澎湃OS融合200+品类，可连接8.2亿设备，全球首创的「人车家全生态」由此大幕开启。

**关于Vela**：[Vela](https://iot.mi.com/vela)是小米公司基于开源实时操作系统NuttX打造的物联网嵌入式软件平台，Vela在各种物联网硬件平台上提供统一的软件服务，支持丰富的组件和易用的框架，用于打通碎片化的物联网应用场景。

**关于NuttX**：[NuttX](https://nuttx.apache.org/docs/latest/)是一个在IoT、分布式嵌入式系统、无人机系统中广泛使用的RTOS，第一个版本由Gregory Nutt于2007年发布。NuttX可以支持8位到64位的处理器，支持risc-v，arm，mips，x86等主流芯片平台，按照POSIX和ANSI标准进行设计，支持MMU和MPU，支持多线程和进程。2019年NuttX在小米的推动下正式进入Apache基金会，小米多位资深工程师参与了NuttX社区的开发和架构设计。经过多年的不懈努力，NuttX功能丰富，性能稳定，商业化成熟度高，在各种物联网产品上得到了广泛的应用。

### 项目意义

Rust是一门系统编程语言，专注于安全，尤其是并发安全，支持函数式和命令式以及泛型等编程范式的多范式语言。Rust在语法上和C++类似，但是在保证性能的同时会提供更好的内存安全机制。当前，Rust语言已经逐步成为Linux内核的基础开发语言之一，后续将在Linux内核的开发中发挥重要作用，并会在后续的系统软件的开发中起到重要作用。

## 预期目标

以Vela平台和NuttX实时操作系统为软件平台基础，结合大赛所提供的K210硬件平台（NuttX RTOS已经完整支持K210板卡），仿照Linux内核的实现方式，对NuttX操作系统进行增强，扩展各种Rust支持。

- 仿照Linux内核的实现，完成NuttX整体Rust支持框架包括编译框架，可以加载和执行模块和应用
- 编写示例的Rust驱动程序，可以加载内核驱动到NuttX内核并运行
- 编写示例的Rust应用程序，可以在NuttX中进行加载和执行
- 利用Rust重写NuttX中的某个子系统框架，并能正常使用和运行

注：上面的内容是建议内容，不要求必须全部完成。所有功能点应能在K210板卡上运行并演示

## 特征

- 文档、代码、问题开放和开源
- 支持K210开发板（基于K210处理器 RV64 CPU）

## 已有参考资料

### 参考文档

- [https://nuttx.apache.org/docs/latest/](https://nuttx.apache.org/docs/latest/) ：NuttX的最新文档，可以直接下载并按照要求配置和使用K210板卡

- https://github.com/apache/incubator-nuttx/tree/master/boards/risc-v/k210/maix-bit ：NuttX文档中对K210板卡的配置和使用说明

- https://security.googleblog.com/2021/04/rust-in-linux-kernel.html

### 参考代码

- https://github.com/apache/nuttx ：目前NuttX针对K210板卡具备完整支持，参赛者可在此基础上进行后续开发

- https://github.com/Rust-for-Linux/linux ：Linux内核的Rust支持

## 赛题分类

内核完善

## 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生或研究生
- 允许学生参加大赛的多个不同题目，最终自己选择一个题目参与评奖
- 请遵循“2024全国大学生操作系统比赛”的章程和技术方案要求

## 难度

中等~高等

## License

Apache 2.0 License

## 所属赛道

2024全国大学生操作系统比赛的“OS功能挑战”赛道

## 项目导师

- 姓名：陈小义
- 单位：小米
- email：[chenxiaoyi@xiaomi.com](mailto:chenxiaoyi@xiaomi.com)
