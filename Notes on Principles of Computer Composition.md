# 计算机组成原理笔记

## 1.1 计算机系统简介  
- 计算机的软硬件概念  
  
- 1.计算机系统
> 计算机系统
> > 硬件：计算机的实体，如主机，外设等  
> > 软件：由具有各类特殊功能的信息(程序)组成

软件：
> 系统软件：用来管理整个计算机系统
- 语言处理程序  
- 操作系统  
- 服务性程序
- 数据库管理系统
- 网络软件
> 应用软件：按任务需要编制成的各种程序

简单的一个层次结构  
| 软件  | 应用软件 | 系统软件 |
| :---: | :------: | :------: |
| 硬件  | 


 **计算机系统的层次结构**
- 系统复杂性管理的方法-1
- 把一个非常复杂的计算机系统用一个简单的层次结构来进行表述，通过封装，我们可以分层来实现一个复杂的计算机系统，当然在分层过程中，我们要处理好各层之间的结构。
- 抽象:
  - 对于一个过程或者一件制品的某些细节有目的的隐藏，以便把其他方面、细节或者结构表达的更加清楚 ——百度百科
  - 指高级的模型，和低级的实体相对 ——维基百科
  - 隐藏系统中不重要的细节  ——David Harris

![计算机层次结构](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number1.png)

![软硬件区分](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number2.png)

- ### 计算机组成与计算机体系结构从研究内容上来说有什么区别？
- 计算机体系结构：程序员所见到的计算机系统的属性概念性和结构与功能特性  例如：有无乘法指令
  - (指令系统、数据类型、寻址技术、I/O机理)
- 计算机组成：实现计算机体系结构所体现的属性  例如：如何实现乘法指令
  - (具体指令的实现) 

1.2 计算机的基本组成
- 一、冯·诺依曼计算机的特点
  - 1. 计算机由五大部分组成
  - 2. 指令和数据以同等地位存于存储器，可按地址寻址
  - 3. 指令和数据用二进制表示
  - 4. 指令由操作在吗和地址码组成
  - 5. **存储程序**
  - 6. 以运算器为中心
![冯·诺依曼计算机硬件框图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number3.png)

- 二、计算机硬件框图
  - 1. 以存储器为中心的计算机硬件框图
  - ![例图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number4.png)
  - 2. ![现代计算机硬件框图-层次化结构](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number5.png)
    - 系统复杂性管理的方法2(3`Y)
      - 层次化(Hierarchy): 将被设计的系统划分为多个模块或子模块 
      - 模块化(Modularity)：有明确定义(well-defined)的功能和结构
      - 规则性(regulariry)：模块更容易被重用

- 三、计算机的工作步骤
  - 1. 上机前的准备
    - 建立数学模型
    - 确定计算方法
    - 编制解题程序
      - 程序 —— 运算的全部步骤
      - 指令 —— 每一个的步骤

![编程举例](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number6.png)

-  **计算机的解题过程**
  - (1) ![存储器的基本组成](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number7.png)
  - **存储体** - **存储单元** - **存储元件** (0/1)
  - 例:大楼 - 房间 - 床位 (无人/有人)
  - 存储单元: 存放和一串二进制代码
  - 存储字: 存储单元中二进制代码的组合
  - 存储字长: 存储单元中二进制代码的位数
    - 每个存储单元赋予一个地址码
  - 存储体按地址寻访
  - (2) **存储器的基本组成**
    - MAR: 存储器地址寄存器 ——反映存储单元的个数
    - MDR: 存储器数据寄存器 ——反映存储字长
    - 例: 设MAR = 4位,MDR - 8位，存储单元个数18位，存储字长8
    - **每个存储单元保存的01个数称为存储字长**
    - **每个存储单元之中保存的数据，称为存储字**
  - **运算器的结构** 
    - 运算器的基本组成及操作过程
      - ![运算器组成](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number8.png)
      - ![操作过程](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number9.png)
      - ![加法操作过程](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/number10.png)
      - ![减法操作过程](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/11.png)
      - ![乘法操作过程](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/12.png) --M 和 ACC 可以同时进行。
      - ![除法操作过程](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/13.png)
   - 控制器的基本结构
     - 控制器的功能:
       - 解释指令
       - 保证指令的按序执行
     - ![完成一条指令](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/14.png)
     - ![控制器的基本组成](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/15.png)
     - PC:程序计数器
       - 存放当前欲执行指令的地址，具有计数功能(PC)+1 ——> PC
     - IR:指令寄存器
       - 存放当前欲执行的指令
     - CU:控制单元
   - 运算器、控制器、存储器构成了什么？
     - 一条指令在主机上的完成过程
     - 程序在主机上是如何执行的
   - 主机完成一条指令的过程
     - ![以取数指令为例](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/16.png)
     - ![取数指令结果](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/17.png)
   - ![存数指令](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/18.png)
   - ax² + bx² + c 程序的运行过程
     - 将程序通过输入设备送至计算机
     - 程序首地址 ——> PC
     - 启动程序运行
     - 取指令 PC ——> MAR ——> M ——> MDR ——> IR
     - 分析指令 **OP**(IR) ——> CU  **OP**--IR操作码的标识  //(PC) + 1 ——> PC 完成乘法指令
     - 执行指令 Ad(IR) ——> MAR ——> M ——> MDR ——> ACC  --**Ad**是IR操作码的标识
     - **循环
     - 打印结果
     - 停机
   - 如果打算买一台机器，如何进行合适的选择？
     - 买这台机器做什么
     - 你有多少钱
     - 机器的性能能否满足你的要求
       > 如何在购买前对计算机的性能进行评价
       > > 处理速度快，内存容量大
   - 计算机硬件的主要技术指标  
    1. 机器字长
      > CPU一次能处理数据的位数
      > > 与CPU中的 **寄存器位数** 有关
   - 运算速度
    > 主频
    > 核数，每个核支持的线程数
    > 吉普森法 ![吉普森法](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/19.png)
    > CPI 执行一条指令所需时钟周期数
    > MIPS 每秒执行百万条指令
    > FLOPS 每秒浮点数运算次数 --从机器能做多少操作的角度进行衡量
  - 存储容量 --存放二进制信息的总位数
    - 主存容量
      - 存储单元个数 x 存储字长
       > 如 MAR MDR 容量
        > > ![图例](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/20.png)
        - 字节数
        - - ![例图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/21.png)
      - 辅存容量
        - 例:字节数 80GB
        - 1GB = 2 $30$B
  ## 计算机的发展及应用
   - 计算机的发展史
     - 计算机的产生和发展
       - 1946年 美国 ENIAC
       - 十进制运算
       - 18000 多个电子管
       - 1500 多个继电器
       - 150 千瓦
       - 30 吨
       - 1500 平方英尺
       - 5000 次加法/秒