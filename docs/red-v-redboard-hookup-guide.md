# RED-V RedBoard 连接指南

> 原文：<https://learn.sparkfun.com/tutorials/red-v-redboard-hookup-guide>

## 介绍

SparkFun 很高兴地欢迎一个全新的指令集架构(ISA)加入其家族，RISC-V ISA ( *读作“风险五”*)，并与它一起推出 [RED-V RedBoard](https://www.sparkfun.com/products/15594) ( *读作“红色五”*)。在本教程中，我们将重点关注硬件。

[![SparkFun RED-V RedBoard - SiFive RISC-V FE310 SoC](img/82e4a4f0f5730309fd75768534852c9c.png)](https://www.sparkfun.com/products/15594) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [spark fun RED-V RED board-SiFive RISC-V Fe 310 SoC](https://www.sparkfun.com/products/15594)

[Out of stock](https://learn.sparkfun.com/static/bubbles/ "out of stock") DEV-15594

SparkFun 的 RED-V RedBoard 是一款低成本、兼容 Arduino 的开发板，采用 Freedom E310，可带来……

$42.958[Favorited Favorite](# "Add to favorites") 17[Wish List](# "Add to wish list")** **[https://www.youtube.com/embed/JnCYY3x26wo/?autohide=1&border=0&wmode=opaque&enablejsapi=1](https://www.youtube.com/embed/JnCYY3x26wo/?autohide=1&border=0&wmode=opaque&enablejsapi=1)

*"The force is strong with this one." (Star Wars: A New Hope, 1977)*

RISC-V ISA 与其他产品的不同之处在于它是完全开源的；包括[指令集架构](https://en.wikipedia.org/wiki/Instruction_set_architecture) (ISA)。这意味着任何人都可以充分利用微控制器，而不需要版税、许可证或保密协议(NDA)。RED-V 采用熟悉的 Arduino Uno 外形，包括 SiFive Freedom E310 内核、32MB QSPI 闪存、用于 USB 连接并作为 JTAG 接口运行的恩智浦 K22 ARM Cortex-M4 以及 Qwiic 连接器。

### 所需材料

要跟随本教程，您将需要以下材料和软件。你可能不需要所有的东西，这取决于你拥有什么。将它添加到您的购物车，通读指南，并根据需要调整购物车。以下是您需要开始的内容:

[![SparkFun RED-V RedBoard - SiFive RISC-V FE310 SoC](img/d3a0ac7c7ca7af0a87e7c0cabca8fbda.png)](https://www.sparkfun.com/products/15594) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [spark fun RED-V RED board-SiFive RISC-V Fe 310 SoC](https://www.sparkfun.com/products/15594)

[Out of stock](https://learn.sparkfun.com/static/bubbles/ "out of stock") DEV-15594

SparkFun 的 RED-V RedBoard 是一款低成本、兼容 Arduino 的开发板，采用 Freedom E310，可带来……

$42.958[Favorited Favorite](# "Add to favorites") 17[Wish List](# "Add to wish list")****[![USB 3.1 Cable A to C - 3 Foot](img/b8f80ffe26048d5be8d999f1de022e13.png)](https://www.sparkfun.com/products/14743) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [USB 3.1 线 A 到 C - 3 脚](https://www.sparkfun.com/products/14743)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") CAB-14743

USB C 棒极了。但是，在我们将所有的集线器、充电器和端口转换为 USB C 之前，这是您要使用的电缆…

$5.504[Favorited Favorite](# "Add to favorites") 9[Wish List](# "Add to wish list")**** *****   红色-V -你肯定需要这个；否则，你很可能在错误的教程页面(*眨眼*)。
*   [USB 3.1 电缆 A 至 C - 3 脚](https://www.sparkfun.com/products/14743)-USB 接口有两个用途:它为电路板供电，并允许您向电路板上传程序。(*你的抽屉里可能会有一些这样的东西！*)

#### 你还需要

要利用开发板的所有功能，您可能需要以下工具和附件。如果您想修改板上的跳线，您将需要[焊接设备](https://www.sparkfun.com/categories/49)。

[![Weller WLC100 Soldering Station](img/740263a3991f953396597751f94187ff.png)](https://www.sparkfun.com/products/14228) 

### [威勒 WLC100 焊台](https://www.sparkfun.com/products/14228)

[Out of stock](https://learn.sparkfun.com/static/bubbles/ "out of stock") TOL-14228

Weller 的 WLC100 是一款多功能的 5 瓦至 40 瓦焊台，非常适合业余爱好者、DIY 爱好者和学生。…

2[Favorited Favorite](# "Add to favorites") 17[Wish List](# "Add to wish list")[![Solder Lead Free - 100-gram Spool](img/7b08ea50c5c651e0ff07ff059946777a.png)](https://www.sparkfun.com/products/9325) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [无铅焊料- 100 克线轴](https://www.sparkfun.com/products/9325)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") TOL-09325

这是带有水溶性树脂芯的无铅焊料的基本线轴。0.031 英寸规格，100 克。这是一个好主意…

$9.957[Favorited Favorite](# "Add to favorites") 33[Wish List](# "Add to wish list")****[![Chip Quik No-Clean Flux Pen  - 10mL](img/a144551d1c264ec16cc42ffeec93ceae.png)](https://www.sparkfun.com/products/14579) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [芯片快克免清洗助焊剂笔- 10mL](https://www.sparkfun.com/products/14579)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") TOL-14579

这款来自 Chip Quik 的 10 毫升免清洗助焊剂笔非常适合您的所有焊接、脱焊、返工和回流目的！

$8.954[Favorited Favorite](# "Add to favorites") 36[Wish List](# "Add to wish list")**** ****#### 跳线修改

如果您想修改板上的跳线，您将需要[焊接设备](https://www.sparkfun.com/categories/49)。

[![Weller WLC100 Soldering Station](img/740263a3991f953396597751f94187ff.png)](https://www.sparkfun.com/products/14228) 

### [威勒 WLC100 焊台](https://www.sparkfun.com/products/14228)

[Out of stock](https://learn.sparkfun.com/static/bubbles/ "out of stock") TOL-14228

Weller 的 WLC100 是一款多功能的 5 瓦至 40 瓦焊台，非常适合业余爱好者、DIY 爱好者和学生。…

2[Favorited Favorite](# "Add to favorites") 17[Wish List](# "Add to wish list")[![Solder Lead Free - 100-gram Spool](img/7b08ea50c5c651e0ff07ff059946777a.png)](https://www.sparkfun.com/products/9325) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [无铅焊料- 100 克线轴](https://www.sparkfun.com/products/9325)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") TOL-09325

这是带有水溶性树脂芯的无铅焊料的基本线轴。0.031 英寸规格，100 克。这是一个好主意…

$9.957[Favorited Favorite](# "Add to favorites") 33[Wish List](# "Add to wish list")****[![Chip Quik No-Clean Flux Pen  - 10mL](img/a144551d1c264ec16cc42ffeec93ceae.png)](https://www.sparkfun.com/products/14579) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [芯片快克免清洗助焊剂笔- 10mL](https://www.sparkfun.com/products/14579)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") TOL-14579

这款来自 Chip Quik 的 10 毫升免清洗助焊剂笔非常适合您的所有焊接、脱焊、返工和回流目的！

$8.954[Favorited Favorite](# "Add to favorites") 36[Wish List](# "Add to wish list")**** ****#### Qwiic 示例

如果你想按照下面的例子与现实世界互动，你还需要以下物品:

[![SparkFun Qwiic 12 Bit ADC - 4 Channel (ADS1015)](img/3e0547fc15fac45cd6cf8820eaaef4e4.png)](https://www.sparkfun.com/products/15334) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [【spark fun Qwiic 12 位 ADC - 4 通道(ADS1015)](https://www.sparkfun.com/products/15334)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") DEV-15334

SparkFun Qwiic 12 位 ADC 可为您的 Qwiic 启用项目提供四个通道的 I ² C 控制 ADC 输入。

$11.501[Favorited Favorite](# "Add to favorites") 22[Wish List](# "Add to wish list")****[![Qwiic Cable - 100mm](img/9c0ab03ac7f7309276f06174476ff62b.png)](https://www.sparkfun.com/products/14427) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [Qwiic 线缆- 100mm](https://www.sparkfun.com/products/14427)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") PRT-14427

这是一条 100 毫米长的 4 芯电缆，带有 1 毫米 JST 端接。它旨在将支持 Qwiic 的组件连接在一起…

$1.50[Favorited Favorite](# "Add to favorites") 32[Wish List](# "Add to wish list")****[![Magnetic Screwdriver Set (20 Piece)](img/680b6735d9cc38d2cf75d6839840d65e.png)](https://www.sparkfun.com/products/retired/15003) 

### [磁性螺丝刀套装(20 件)](https://www.sparkfun.com/products/retired/15003)

[Retired](https://learn.sparkfun.com/static/bubbles/ "Retired") TOL-15003

这是一个 20 件螺丝刀组，磁性保持每个未使用的位固定在一个薄的情况下，很容易…

1 **Retired**[Favorited Favorite](# "Add to favorites") 12[Wish List](# "Add to wish list")**** ****#### 赛格程序员

如果你想自己调试或刷新你的处理器，这里有一些我们的程序员。我们还建议用一些跳线连接 1.27 毫米的接头引脚。根据您使用的编程器，您可能需要结合使用绕线和 IC 挂钩来连接。

[![Header - 2x5 Pin (Male, 1.27mm)](img/71422aa00fd5e0a63e30c106c758f5ef.png)](https://www.sparkfun.com/products/15362) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [【接头- 2x5 引脚(公，1.27mm)](https://www.sparkfun.com/products/15362)

[In stock](https://learn.sparkfun.com/static/bubbles/ "in stock") PRT-15362

这是一个超小型 2x5 引脚公型 PTH 接头。该标题是 JTAG 应用程序的通用配置。

$1.75[Favorited Favorite](# "Add to favorites") 4[Wish List](# "Add to wish list")****[![J-Link BASE Compact Programmer](img/e1749da991a919e3ecf97f50ac8ecb10.png)](https://www.sparkfun.com/products/15347) 

将**添加到您的[购物车](https://www.sparkfun.com/cart)中！**

### [J-Link BASE 紧凑型编程器](https://www.sparkfun.com/products/15347)

[Only 4 left!](https://learn.sparkfun.com/static/bubbles/ "only 4 left!") PGM-15347

紧凑型 J-Link 编程器，用于对任何 ARM 微控制器进行编程。

$525.95[Favorited Favorite](# "Add to favorites") 4[Wish List](# "Add to wish list")****[![J-Link EDU Mini Programmer](img/95b4a314ecb6ff60bfbff57fabf72c64.png)](https://www.sparkfun.com/products/retired/15345) 

### [J-Link EDU 迷你程序员](https://www.sparkfun.com/products/retired/15345)

[Retired](https://learn.sparkfun.com/static/bubbles/ "Retired") PGM-15345

微型 J-Link 编程器，用于对任何 ARM 微控制器进行编程。附带教育/非商业许可证。

1 **Retired**[Favorited Favorite](# "Add to favorites") 9[Wish List](# "Add to wish list")[![J-Link EDU Base Programmer](img/0dee95f73493b1f50a00f526e28ccfdd.png)](https://www.sparkfun.com/products/retired/15346) 

### [J-Link EDU 基地程序员](https://www.sparkfun.com/products/retired/15346)

[Retired](https://learn.sparkfun.com/static/bubbles/ "Retired") PGM-15346

J-Link 编程器，用于对任何 ARM 微控制器进行编程。附带教育/非商业许可证。

2 **Retired**[Favorited Favorite](# "Add to favorites") 3[Wish List](# "Add to wish list")**** ****### 推荐阅读

在继续本教程之前，如果您不熟悉这些主题，您可能需要熟悉它们。

[](https://learn.sparkfun.com/tutorials/how-to-solder-through-hole-soldering) [### 如何焊接:通孔焊接](https://learn.sparkfun.com/tutorials/how-to-solder-through-hole-soldering) This tutorial covers everything you need to know about through-hole soldering.[Favorited Favorite](# "Add to favorites") 70[](https://learn.sparkfun.com/tutorials/logic-levels) [### 逻辑电平](https://learn.sparkfun.com/tutorials/logic-levels) Learn the difference between 3.3V and 5V devices and logic levels.[Favorited Favorite](# "Add to favorites") 82

## 硬件概述

### 电源和编程

给 SparkFun RED-V RedBoard 供电有几种不同的方式:

*   USB-C
*   筒式插孔连接器
*   主板边缘的电源针脚断裂

最简单的方法(也允许您对您的板进行编程)是简单地通过 USB-C 将其插入您的计算机。这将为板提供 5V 电压，并允许您访问超级酷的 USB 到 JTAG 接口进行编程。然而，一旦你对你的 RED-V 进行了编程，你可能想让它使用不同的电源。如果您在 USB-C 连接器上使用壁式电源插座，请确保它输出经过调节的 **5V DC** 。你也可以使用黑色桶形插孔，在这种情况下，你需要在 **7 & 15 伏 DC** 之间的任何墙壁适配器。或者，您也可以通过电路板边缘的接头引脚为电路板供电。如果您使用的是`VIN`和`GND`，遵循与使用墙壁适配器相同的做法，并保持在 7 & 15 伏之间。如果您正在使用`5V`和`GND`或`3v3`和`GND`，请确保在分别向 5V 或 3.3V 引脚供电时，您的电压是稳定的。

[![USB, Barrel Jack, and Power Pins](img/2c4986e9a830faf94ed9c2d62228976c.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/RED-V_RedBoard_SiFive_RISC-V_FE310_SoC_Power.jpg)

#### 永远在线的核心

FE310 包含一个始终开启(AON)模块，可以轻松控制 FE310 的电源。它包括自己的实时时钟，也连接到板上的`WAKE`按钮。这允许您将 FE310 置于睡眠状态，并在时间或用户产生中断时将其唤醒。

[![FE310 IC](img/7a8b657673306e73d45a931d7caca01e.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/RED-V_RedBoard_SiFive_RISC-V_FE310.jpg)

### 小跟班

红色 V 有两个按钮:一个`RESET`按钮和一个`WAKE`按钮。`RESET`按钮非常简单，用于重置 FE310。点击`RESET`按钮将运行加载到 Fe 310 QSPI 闪存上的代码。快速双击将使 FE310 进入安全引导模式，这将允许您将新代码刷新到 RED-V，如果您真的把事情搞砸了(例如，糟糕，我让内核进入睡眠状态，忘记添加唤醒它的方法)。引脚也在电路板边缘断开。在此引脚和 GND 之间添加一条跳线也会重置电路板。

[![Reset Button and Pin](img/54ee1964c9b727f2ad19a3e6d8d70189.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/RED-V_RedBoard_SiFive_RISC-V_FE310_Reset.jpg)

RED-V 还配备了一个常通或 AON 内核(如上所述),可以通过编程关闭 FE310 的主内核，并在按钮产生或用户产生中断时将其唤醒。可以在软件中配置`WAKE`按钮，将 FE310 从深度睡眠中唤醒。如果您想使用外部电源来唤醒 FE310，此按钮也可用于最靠近桶形插孔的接头引脚。在此引脚和 GND 之间添加一条跳线也会唤醒电路板。

[![Wake Button and Pin](img/e435740b78575336a589b70dd3415831.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/RED-V_RedBoard_SiFive_RISC-V_FE310_Wake.jpg)

### 针织套衫

FE310 也有一些跳线，默认情况下都是打开的。位于`I2C`标签旁边的两个跳线用于 I ² C 上拉电阻。默认情况下不连接这些电阻，因为所有 SparkFun Qwiic 从机上都有 I ² C 上拉电阻。如果你使用 3 ^(rd) party board，你可能需要[闭合 Qwiic 连接器](https://learn.sparkfun.com/tutorials/how-to-work-with-jumper-pads-and-pcb-traces#adding-a-solder-jumper)旁边的这些跳线，以将上拉电阻连接到 I ² C 总线。USB-C 连接器旁边的跳线用于绕过 0.5A PTC 保险丝。这是用于需要大量电流的特殊情况。大多数时候，你可以让这个跳线开着。

[![Pull-Up Resistors and By-Pass jumper](img/c532e5c9275938b8524541aacdd9e3f8.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/RED-V_RedBoard_SiFive_RISC-V_FE310_Jumpers.jpg)

### 规模

RED-V RedBoard 使用 Arduino Uno 封装。板上有四个安装孔。

[![Dimensions](img/21013af044860bf923a20048543e0927.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/SparkFun_RED-V__RedBoard_Dimensions.png)

## 硬件连接

就本教程而言，您将使用 USB C 电缆供电、上传代码并向电路板发送串行信号。只需连接计算机的 USB 端口和 RED-V。该板使用标准的 Arduino Uno R3 封装，带有母头，用于堆叠 Arduino 屏蔽，并通过跳线轻松连接试验板上的原型电路。

[![USB Cable to RED-V](img/3d5df0639ee0c69294b7f3569cc47598.png)](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/RED-V_RedBoard_cable.jpg)**Note:** While the board uses the standard Arduino Uno R3 footprint, keep in mind the board uses [3.3V logic levels](https://learn.sparkfun.com/tutorials/logic-levels/all). Additionally, Arduino shields might have been only developed for an AVR architecture and the Arduino programming language. You may need to put in a little bit more effort to write a library in order to get it working depending on the FE310 and your preferred programming language.

## 软件开发指南

RED-V 有几种入门环境，有关 RED-V RedBoard 编程的信息，请查看以下教程。

[](https://learn.sparkfun.com/tutorials/red-v-development-guide) [### RED-V 开发指南

#### 2019 年 11 月 27 日](https://learn.sparkfun.com/tutorials/red-v-development-guide) This guide will help you get the RED-V RedBoard or Thing Plus up and running for the exhaust port. Depending on personal preference, there are a few environments to get started with the boards. All wings report in... we're going in full-throttle.[Favorited Favorite](# "Add to favorites") 3

## 资源和更进一步

现在你已经成功地开始使用你的 RED-V RedBoard，是时候把它合并到你自己的项目中了！有关更多信息，请查看以下资源:

*   [示意图(PDF)](https://cdn.sparkfun.com/assets/d/d/1/e/7/RedFive.pdf)
*   [老鹰文件(ZIP)](https://cdn.sparkfun.com/assets/6/9/f/0/c/SparkFun_REDV_RedBoard.zip)
*   [尺寸](https://cdn.sparkfun.com/assets/learn_tutorials/1/0/3/2/SparkFun_RED-V__RedBoard_Dimensions.png)
*   [Qwiic 登陆页面](https://www.sparkfun.com/qwiic)
*   [RISC-V](https://riscv.org/)
    *   [规格](https://riscv.org/specifications/)
    *   [软件状态](https://riscv.org/software-status/)
    *   [内核](https://riscv.org/risc-v-cores/)
*   [四五](https://www.sifive.com/)
    *   [E310-G002](https://www.sifive.com/documentation)
        *   [数据表(PDF)](https://cdn.sparkfun.com/assets/5/b/e/6/2/fe310-g002-ds.pdf)
        *   [手册(PDF)](https://cdn.sparkfun.com/assets/7/f/0/2/7/fe310-g002-manual-v19p05.pdf)
    *   [自由工作室和 E SDK](https://www.sifive.com/boards/#software)
    *   [自由工作室用户手册(PDF)](https://cdn.sparkfun.com/assets/learn_tutorials/1/1/0/1/freedom-studio-manual-4.7.2-2019-08-2.pdf)
*   [GitHub 硬件回购](https://github.com/sparkfun/Red_V)
*   [SFE 产品展示区](https://youtu.be/JnCYY3x26wo)**********************