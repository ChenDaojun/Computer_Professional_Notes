**计算机网络的概念**  
- 计算机网络：是一个将分散的、具有独立功能的**计算机系统**，通过**通信设备**与**线路**连接起来，由功能完善的**软件**实现**资源共享**和**信息传递**的系统。
- 计算机网络是**互连**、**自治**的计算机集合 
- 互连-互联互通 通信链路  
- 自治-无主从关系  

**计算机网络的功能**  
1. 数据通信(连通性)
2. 资源共享 硬件 软件 数据
- **以上两大功能是计算机网络最主要的**
3. 分布式处理 多台计算机各自承担同一工作任务的不同部分
4. 提高可靠性
5. 负载均衡

**计算机网络的组成**
1. 组成部分 
    - 硬件、软件、协议
2. 工作方式
    - 边缘部分
        - 用户直接使用
            - C/S方式
            - P2P方式
    - 核心部分 为边缘部分服务
3. 功能组成
    - 通信子网 实现**数据通信**
    - 资源子网 实现**资源共享**/数据处理

![计算机网络组成](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Computer-Network-images(screenshot)/number1.png)
![总结](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Computer-Network-images(screenshot)/number2.png)
**标准化工作**  

标准的分类：
- 法定标准：由权威机构制定的正式的、合法的标准 [OSI]
- 事实标准：某些公司的产品在竞争中占据了主流，时间长了，这些产品的协议和技术就成为了标准

RFC(Fequest For Comments) --因特网标准的形式  
RFC要上升位因特网正式标准的**四个阶段**：
1. 因特网草案(Internet Draft) 这个阶段还不是RFC文档。
2. 建议标准(Proposed Standard) 从这个阶段开始成为RFC文档。
3. _草案标准(Draft Standard) 通过IETF、IAB审核_ (自2011起取消)
4. 因特网标准(Internet Standard)

标准化工作的相关组织
- 国际标准化组织 ISO ：建立OSI参考模型、HDLC协议
- 国际电信联盟 ITU：制定通信规则
- 国际电子电气工程师协会 IEEE：学术机构、IEEE802系列标准、5G
- Internet工程任务组 IETF：负责因特网相关标准的制定 

![思维导图](https://cdn.jsdelivr.net/gh/ChenDaojun/MyCDN/images/Computer-Network-images(screenshot)/number3.png)

---

## 速率
- 速率即 **数据率** 或成 **数据传输率** 或 **比特率**
- 比特 1/0 位
- 连接在计算机网络上的 **主机** 在数字信道上传送数据 **位数的速率**
- 单位是 b/s , kb/s, Mb/s, Gb/s, Tb/s

1. 千 $1kb/s = 10³b/s$
2. 兆 $1Mb/s = 10³kb/s = 10^6b/s$
3. 吉 $1Gb/s = 10³Mb/s = 10^6kb/s = 10^9b/s$
4. 太 $1Tb/s = 10³Gb/s = 10^9kb/s = 10^{12}b/s$