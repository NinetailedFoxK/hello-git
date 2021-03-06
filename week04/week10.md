# 1.[计算机网络出现的背景]

## 1.1 计算机的普及与多样化

> 1. 20世纪最伟大的发明就是计算机
> 2. 计算机应用：
>
> > 1. 较易理解计算机设备：个人电脑、笔记本电脑、平板电脑、手机终端（智能手机）等便携设备
> > 2. 较为隐藏的计算机设备：家用电器、音乐播放器、办公电器、汽车等设备等，芯片由计算机控制
>
> 3. 计算机的演变

## 1.2 从独立模式到网络互连模式

* 计算机以单机模式被广泛使用

> 1. WAN（Wide Area Network,广域网)
> 2. 城域网（MAN，Metropolitan Area Network）

## 1.3 从计算机通信到信息通信

> 1. 私有网络：由管理员将特定的几台计算机相连在一起形成计算机网络
> 2. 互联网：私有网络相互连接组成更大的私有网络 ———— 逐渐实现计算机之间的通信

## 1.4 计算机网络的作用

* 随着互联网爆发性地发展与普及，信息网络已随处可见。

```
社团成员、学校同窗之间可以通过邮件组（使用电子邮件实现公告板的功能。
所有订阅该邮件组的成员都可以收到发送给该组的邮件。） 、主页、
BBS论坛相互联系，甚至可以通过网络日志（以文本为中心的主页或服
务。用户可以像写日记一样很方便地更新内容。） 、聊天室、即时通
信以及SNS（社交网络。指由一群个人或团体在互联网上组成的关系网
络。通过SNS，人们可以发布自己近期的活动、生活感想以及最新作
品，让圈内成员实时掌握个人动态。） 实现互联与信息互换。
```



# 2. [计算机与网络发展的7个阶段]

> 1. 批处理
> 2. 分时系统
> 3. 计算机之间的通信
> 4. 计算机网络的产生
> 5. 互联网的普及
> 6. 以互联网技术为中心的时代
> 7. 从“单纯建立连接”到“安全建立连接”
> 8. 手握金刚钻的TCP/IP

------



# 3. [协议]


* 现实世界是有规律的，一切都在规定的规则下按部就班的进行。如果没有规则，混乱即将来临。虚拟世界亦是如此

* [TCP/IP到底是个啥？](https://www.bilibili.com/video/BV1hs411v7Zx?from=search&seid=15244659118069254908&spm_id_from=333.337.0.0)
* TCP/IP就是IP、TCP、HTTP等协议的集合（大概有100多种）

## 1. 随处可见的协议

> 1. 互联网： IP、TCP、HTTP
> 2. 局域网：IPX/SPX 

## 2. 协议的必要性

```
协议就是计算机与计算机之间通过网络实现通信时事先
达成的一种“约定”。这种“约定”使那些由不同厂商的设备、不同的CPU
以及不同的操作系统组成的计算机之间，只要遵循相同的协议就能够实
现通信。
```

## 3. 协议如同人与人的对话

* 将汉语和英语当作“协议”
* 将聊天当作“通信”
* 将说话的内容当作“数据”

## 4. 计算机中的协议

* 在计算机通信中，事先达成一个详细的约定，并遵循这一约定进行处理尤为重要。这种约定其实就是“协议”。

## 5. 分组交换协议



# 4. [协议由谁规定]

## 1. 协议的标准化




# 5. [协议分层与OSI参考模型]

![](https://ts1.cn.mm.bing.net/th/id/OIP-C.7-iwxpmr8-0iGCl-qYEywAHaGY?pid=ImgDet&rs=1)

## 1. 协议的分层

### 1. 分层的优势

> 1. 独立性：分层可以将每个分层独立使用，即使系统中某 些分层发生变化，也不会波及整个系统
> 2. 扩展性
> 3. 灵活性
> 4. 细分功能：通过分层能够细分通信功能，更易于单独 实现每个分层的协议，并界定各个分层的具体责任和义务

### 2. 分层的劣势

> 1. 过于模块化
> 2. 使处理变得更加沉重
> 3. 每个模块都不得不实现相似的处理逻辑

<img src="typora-user-images/image-20211109211143223.png" alt="image-20211109211143223" style="zoom:40%;" />

## 2. 通过对话理解分层

![image-20211109211245344](typora-user-images/image-20211109211245344.png)







## 3. OSI参考模型

<img src="https://images.gitee.com/uploads/images/2021/1109/200617_745b90e4_4961328.png" width=60% />

## 4. OSI参考模型中各个分层的作用

[互联网是如何工作的？DNS、MAC、IP地址都是啥？](https://www.bilibili.com/video/BV1VE41187N7?from=search&seid=16481405030413792793&spm_id_from=333.337.0.0)



<img src="typora-user-images/image-20211109211546255.png" alt="image-20211109211546255" style="zoom:50%;" />

# 6. [**OSI**参考模型通信处理举例]



## 案例：A的用户A要 给使用主机B的用户B发送一封电子邮件



### 1. 会话层以上的处理：

> 1. **应用层**
>
> >```mermaid
> >graph TB
> >C[client客户段]--首部+早上好-->S[Server服务端]
> >```
>
> 2. **表示层**：表示层的“表示”有“表现”、“演示”的意思，因此更关注数据的具体 **表现形式 **。
>
> > ```mermaid
> > graph TB
> > a[某个计算机特定的数据格式]-->b[网络通用的标准数据格式]-->c[数据恢复:该计算机特定的数据格式]
> > ```
> >
> > * 数据格式: 以中文编码格式为例：
> >   [常见中文编码格式](https://blog.csdn.net/u010009033/article/details/81103334)
>
> > 1. Unicode编码
> > 2. UTF-8编码
> > 3. GB2312编码
> > 4. BIG5编码
> > 5. GBK编码
> > 6. GB18030编码
> >
> > * 如果未能按照特定格式编码，那么在 接收端就是收到邮件也可能会是乱码

> 3. **会话层**
>
> > * 采用何种方式进行传输数据
> >
> >   ![image-20211109215852623](typora-user-images/image-20211109215852623.png)
>
> > ```
> > 假定用户A新建了5封电子邮件准备发给用户B。这5封邮件的发送 顺序可以有很多种。例如，可以每发一封邮件时建立一次连接(指通信 连接。) ，随后断开连接。还可以一经建立好连接后就将5封邮件连续 发送给对方。甚至可以同时建立好5个连接，将5封邮件同时发送给对 方。决定采用何种连接方法是会话层的主要责任。
> > ```

### 2. 传输层以下的处理

* 4.**传输层**

  ![image-20211109215829168](typora-user-images/image-20211109215829168.png)

* 数据链路层、物理层

  ![image-20211109220406675](typora-user-images/image-20211109220406675.png)



# 7. [传输方式的分类]

## 1. 面向有连接型与面向无连接型

* 面向有连接型

* 面向无连接型

  ![image-20211109221243715](typora-user-images/image-20211109221243715.png)

## 2.  电路交换与分组交换

* 1. 电路交换：如电话网
* 2. 分组交换：如TCP/IP

* 阅读、讨论与思考：上述两种方式的不同有哪些？分组交换的优势是什么？可能风险是什么？



## 3. 根据接收端数量分类

> 1. 单播(**Unicast**)
> 2. 广播(**Broadcast**)
> 3. 多播(**Multicast**)
> 4. 任播(**Anycast**)

![image-20211110000516326](typora-user-images/image-20211110000516326.png)



# 8. 地址



## 1. 地址的唯一性





## 2. 地址的层次性



# 9. 网络的构成要素



## 1. 通信媒介与数据链路





## 2. 网卡



## 3. 中继器

* 中继器(Repeater)是在OSI模型的第1层——物理层面上延长网络 的设备

* 核心功能：网络信号放大

* > ![image-20211110003418791](typora-user-images/image-20211110003418791.png)

## 4. 网桥**/2**层交换机



## 5. 路由器**/3**层交换机



## 6. **4**~**7**层交换机



## 7. 网关





