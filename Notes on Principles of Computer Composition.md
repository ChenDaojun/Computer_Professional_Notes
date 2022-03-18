# 计算机组成原理笔记
- [计算机组成原理笔记](#计算机组成原理笔记)
  - [第一章 计算机系统简介](#第一章-计算机系统简介)
  - [第二章 计算机的发展及应用](#第二章-计算机的发展及应用)
  - [第三章 系统总线](#第三章-系统总线)
  - [第四章 存储器](#第四章-存储器)
## 第一章 计算机系统简介  
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
- --
  ## 第二章 计算机的发展及应用
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
     - ![世界上第一台计算机 ENIAC(1946)](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/22.png)
     - 现代计算机产生的驱动力
       - 需求，需求，还是需求
       - 技术发展
         - 电子技术的发展
         - 计算机体系结构技术的发展
       - 硬件技术对计算机更新换代的影响
     - ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/23.png)
     - ![von Neumann系统结构的计算机](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/24.png)
     - ![IAS的逻辑结构](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/25.png)
     - ![IBM 360照片](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/26.png)

     - 微型计算机的出现和发展
      - 微处理器芯片  ——1971年，由Intel公司开发
        - 4位(4004)
        - 8位
        - 16位
        - 32位
        - 64位
      - 存储器芯片  ——1970年
        - 256位
        - 1k位
        - 4k位
        - 16k位
        - 64k位
        - 256k位
        - 1M位
        - 4M位
        - 16M位
        - 64M位
      - ![Intel公司典型的微处理器产品](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/27.png)
      - Moore 定律
        - Intel公司的缔造者之一，Gordon Moore提出
        - 微芯片上集成的晶体管数目每三年翻两番
        - 每隔18个月番一番，性能提升一倍
     - 三、软件技术的兴起和发展
      - 各种语言
        - 机器语言  面向机器
        - 汇编语言  面向机器
        - 高级语言  面向问题
          - FORTRAN 科学计算和工程计算
          - PASCAL 结构化程序设计
          - C++  面向对象
          - Java 适应网络环境
      - 系统软件
        - **语言处理程序**  汇编程序 编译程序
        - 操作系统  DOS、UNIX、Windows、Linux、Kylin Linux
        - 服务性程序 装配 调试 诊断 排错
        - 数据库管理系统 数据库和数据库管理软件
        - 网络软件
      - 软件发展的特点
        - 开发周期长
        - 制作成本昂贵
        - 检测软件产品质量的特殊性
        - 软件是程序以及开发、使用和维护程序所需要的所有文档
      - 计算机的应用
        - 科学计算和数据处理
        - 工业控制和实时控制
        - 网络技术
          - 电子商务
          - 网络教育
          - 敏捷制造
        - 虚拟现实
        - 办公自动化和管理信息系统
        - CAD/CAM/CIMS
          - CAD: 计算机辅助设计
          - CAM: 计算机辅助制造
          - CIMS: 计算机集成制造系统
        - 多媒体技术
        - 人工智能
      - 计算机的展望
        - 一、计算机具有类似人脑的一些超级智能功能
          - 要求计算机的速度要足够快
        - 二、芯片集成度的提高受以下三方面的限制
          - 芯片集成度受物理极限的制约
          - 按几何级数递增的制作成本
          - 芯片的功耗、散热、线延迟
        - 三、替代传统的硅芯片
          - 光计算机
            - 利用光子取代电子进行运算和存储
          - DNA生物计算机
            - 通过控制DNA分子间的生化反应
          - 量子计算机
            - 利用原子所具有的量子特性

---

## 第三章 系统总线
 3.1 总线的基本概念  
 3.2 总线的分类  
 3.3 总线特征及性能指标  
 3.4 总线结构  
 3.5 总线控制  

  - 3.1 总线的基本概念
    - 一、为什么要用总线？
    - 二、什么是总线
      - 总线是连接各个部件的信息传输线，是 **各个部件共享的传输介质**
    - 三、总线上信息的传送
      - 串行 一串的一串的传输，一串一串的接收
      - 并行 多串同时传输，同时接收
    - 四、总线结构的计算机举例
    - 1、单总线结构框图
      - ![单总线](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/28.png)
    - 2、面向 CPU 的双总线结构框图
      - ![以CPU为主的双总线](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/29.png)
    - 3、以存储器为中心的双总线结构框架
      - ![以存储器为主的双总线](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/30.png)
      
  - 3.2 总线的分类
    - 1.片内总线  芯片内部的总线
    - 2.系统总线  **计算机各部件之间** 的信息传输线
      - 数据总线  **双向** 与机器字长、存储字长有关
      - 地址总线  **单向** 与存储地址、I/O地址有关
      - 控制总线  **有出** **有入**
        - 有出: 存储器读、存储器写、总线允许、中断确认
        - 有入:中断请求、总线请求
    - 3.通信总线
      - 用于 **计算机系统之间** 或 **计算机系统与其他系统** (如控制仪表、移动通信等) 之间的通信
        - 传输方式:**串行通信总线** 或 **并行通信总线**
  - 3.3 总线特性及性能指标
    - 一、总线物理实现
      - ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/31.png)
    - 二、总线特性
      - 1.机械特性  **尺寸**、形状、**管脚数** 及 **排列顺序**
      - 2.电气特性  **传输方向** 和有效的 **电平** 范围
      - 3.功能特性  每根传输线的 **功能**
        - 地址
        - 数据
        - 控制
      - 4.时间特性  信号的 **时序** 关系
    - 三、总线的性能指标
      - 1.总线宽度  **数据线** 的根数
      - 2.标准传输率  每秒传输的最大字节数(**MBps**)
      - 3.时钟同步/异步  **同步**、**不同步**
      - 4.总线复用  **地址线** 与 **数据线** 复用
      - 5.信号线数  地址线、数据线和控制线的 **总和**
      - 6.总线控制方式  突发、自动、仲裁、逻辑、计数
      - 7.其他指标  **负载能力**
    - 四、总线标准
      - 标准界面 多个模块或系统同时遵守的标准
      - 总线标准 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/32.png)
  - 3.4 总线结构
    - 一、单总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/33.png) 
    - 二、多总线结构 
    - 1.双总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/34.png)
    - 2.三总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/35.png)
    - 3.三总线结构的又一形式 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/36.png)
    - 4.四总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/37.png)
    - 三、总线结构举例
    - 1.传统微型机总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/38.png)
    - 2.VL-BUS局部总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/39.png)
    - 3.PCI总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/40.png)
    - 4.多层 PCI 总线结构 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/41.png)
  - 3.5 总线控制
    - 一、总线判优控制
      - 1.基本概念
        - 主设备(模块)  对总线有 **控制权**
        - 从设备(模块)  **响应** 从主设备发来的总线命令
        - 总线判优控制
          - 集中式 
            - 链式查询
            - 计数器定时查询
            - 独立请求方式
          - 分布式
      - 2.链式查询方式 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/42.png)
      - 3.计数器定时查询方式 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/43.png)
        ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/44.png)
      - 4.独立请求方式 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/45.png)
    - 二、总线通信协议
      - 1.目的  解决通信双方 **协调配合** 问题
      - 2.总线传输周期
        - 申请分配阶段  **主模块申请**，总线仲裁决定 
        - 寻址阶段  主模块向从模块 **给出地址** 和 **命令**
        - 传数阶段  主模块 和 从模块 **交换数据**
        - 结束阶段  主模块 **撤销有关信息** 同时从模块也撤销
      - 3.总线通信的四种方式
        - 同步通信  由 **统一时标** 控制数据传送
        - 异步通信  采用 **应答方式**，没有公共时钟标准
        - 半同步通信  同步、**异步结合**
        - 分离式通信  充分 **挖掘** 系统 **总线每个瞬间** 的潜力
        - (1)同步式数据输入 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/46.png)
        - (2)同步式数据输出 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/47.png)
        - (3)异步通信 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/48.png)
        - (4)半同步通信(同步、异步结合)
          - 同步  **发送方** 用系统 **时钟前沿** 发信号
          - **接收方**  用系统 **时钟后沿** 判断、识别
          - 异步  允许不同速度的模块和谐工作
          - 增加一条 **“等待”响应信号**  WAIT信号(等待信号)
          - ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/49.png)
        - **以输入数据为例的半同步通信时序**
          - T1 主模块发地址
          - T2 主模块发命令
          - Tw 当 WAIT 为低电平时，等待一个T
          - Tw 当 WAIT 为低电平时，等待一个T
          - ...
          - T3 从模块提供数据
          - T4 从模块撤销数据，主模块撤销命令
        - 上述三种通信的共同点
        - **一个总线传输周期**(**以输入数据为例**)
          - 主模块发地址、命令  **占用总线**
          - 从模块准备数据  **不占用总线**  总线空闲
          - 从模块向主模块发数据  **占用总线**
        - (5)分离式通信
          - **充分挖掘系统总线每个瞬间的潜力**
          - 一个总线传数周期
          - 分成两个子周期
            - 子周期1  **主模块** 申请 **占用总线**，使用完后即 **放弃总线** 的使用权
            - 子周期2  **从模块**(从模块可变成主模块) 申请 **占用总线**，将各种信息送至总线上
            - 分离式通信特点
              - 1.各模块有权申请占用总线
              - 2.采用同步方式通信，不等对方回答
              - 3.各模块准备数据时，不占用总线
              - 4.总线被占用时，无空闲

---

## 第四章 存储器
 4.1 概述
  - 存储器可分哪些类型？
  - 现代存储器的层次架构，为什么要分层？
 
---

  - **4.1** 概述
    - 一、**存储器分类**
    - 1.**按存储介质分类**
      - (1)半导体存储器  TTL、MOS  **易失**
      - (2)磁表面存储器  磁头，载磁体
      - (3)磁芯存储器  硬磁材料、环状元件
      - (4)光盘存储器  激光、磁光材料
      - 以上三个都是非易失
    - 二、按存取方式分类
      - (1)存取时间和物理地址无关(随机访问)
        - 随机存储器  **在程序的执行过程中** 可 **读** 可 **写**
        - 只读存储器  **在程序的执行过程中** **只读**
      - (2)存取时间与物理地址有关(串行访问)
        - 顺序存取存储器  磁带
        - 直接存取存储器  磁盘
    - 3、按在计算机中的作用分类
      - 存储器
        - 主存储器
          - RAM
            - 静态RAM
            - 动态RAM
          - ROM
            - MROM
            - PROM
            - EPROM
            - EEPROM
        - Flash Memory
        - 高速缓冲存储器 (Cache)
        - 辅助存储器  磁盘、磁带、光盘
    - 三、存储器的层次结构
      - 1.存储器三个主要特征的关系 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/50.png)
      - 速度由快到慢
      - 容量从小到打
      - 价格从高到低
      - 2.缓存——主存层次和主存——辅存层次 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/51.png)
      - ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/52.png)
      - ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/53.png)
      - 缓存 —— 主存  (容量)
      - 主存 —— 辅存  (速度)
        - 虚拟存储器 
        - 虚地址
        - 逻辑地址
      - 主存储器用到的地址
        - 实地址
        - 物理地址


  - 4.2 **主存储器**——概述
  - 
  - 1.主存的基本组成
  - 2.主存和CPU之间的联系
  - 3.主存中存储单元地址的分配
  - 4.主存的技术指标
    
    - 一、概述
      - 1.主存的基本组成 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/54.png)
      - 2.主存和CPU的联系 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/55.png)
      - 3.主存中存储单元地址的分配 
        - 12345678H 这个数据如何在 **主存储器中进行存储？**
        - **高位字节** ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/56.png)
        - **低位字节** 地址为字地址  ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/57.png)
        - 设地址线 **24** 根  按 **字节** 寻址 $2^{24}$
        - 若字长为 **16** 位  按 **字** 寻址  8MW  W即word，字
        - 若字长 **32** 位  按 **字** 寻址  4MW
      - 4.主存的技术指标
        - (1)存储容量  **主存** **存放二进制代码的总位数**
        - (2)存储速度  
          - 存取时间  存储器的 **访问时间**  
            - 读出时间 写入时间
          - 存取周期  **连续两次独立的存储器操作**
            - (读或写) 所需的 **最小间隔时间**
            - 读周期  写周期
          - (3)存储器的带宽  **位**/**秒**

  - 4.2 主存储器 ——半导体芯片简介
    - 1.半导体存储芯片的基本结构
    - 2.半导体存储芯片的译码驱动方式
      - 线选法
      - 重合法

      1.半导体存储芯片的基本结构  ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/58.png)
      ![片选线](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/59.png)
      - 存储芯片片选线的作用
        - 用 16k x 1位 的存储芯片组成 64k x 8位 的存储器  ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/60.png)
      2.半导体存储芯片的译码驱动方式
      - (1)线选法 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/61.png)
      - (2)重合法 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/62.png)

  - 4.2 主存储器 ——随机存取存储器
    - 1.**静态RAM**(**SRAM**)
      - 保存 0 和 1 的原理是什么？
      - 基本单元电路的构成是什么？
      - 对单元电路如何读出和写入？
      - 典型芯片的结构是什么样子的？
      - 静态RAM芯片是如何进行读出和写入操作？
    - 2.**动态RAM**(**DRAM**)
    - 3.**动态RAM** 和 **静态RAM** 的比较
    
    - 三、随机存取存储器(RAM)
      - 1.静态RAM(SRAM)
        - (1)静态RAM基本电路 ![图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Notes-on-Principles-of-Computer-Composition/63.png)