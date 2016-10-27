## ZigBee

　**ZigBee**（也称紫蜂）是一种低速短距离传输的无线网络协议，底层是采用IEEE 802.15.4标准规范的媒体访问层与物理层。主要特色有低速、低耗电、低成本、支持大量网络节点、支持多种网络拓扑、低复杂度、快速、可靠、安全。

## IEEE802.15.4/ZigBee协议概述

IEEE802.15.4协议是IEEE802.15.4工作组为低速率无线个人区域网（**WPAN:Wireless Personal Area Network**）制定的标准，该工作组成立于2002年12月，致力于定义一种廉价的，固定、便携或移动设备使用的，低复杂度、低成本、低功耗、低速率的无线连接技术，并于2003年12月通过了第一个802.15.4标准。随着无线传感器网络技术的发展，无线传感器网络的标准也得到了快速的发展。802.15.4标准定义了在个人区域网中通过射频方式在设备间进行互连的方式与协议，该标准使用避免冲突的载波监听多址接入以方式作为媒体访问机制，同时支持星型与对等型拓扑结构。

在802.15.4标准中指定了两个物理频段和直接序列扩频（**DSSS**）物理层频段：868/915MHz和2.4GHz。2.4GHz的物理层支持空气中250kb/s的速率，而868/915MHz的物理层支持空气中20kb/s和40kb/s的传输速率。由于数据包开销和处理延迟，实际的数据吞吐量会小于规定的比特率。作为支持低速率、低功耗、短距离无线通信的协议标准，802.15.4在无线电频率和数据率、数据传输模型、设备类型、网络工作方式、安全等方面都做出了说明。并且将协议模型划分为物理层和媒体接入控制层两个子层进行实现。

ZigBee协议是由ZigBee联盟制定的无线通信标准，该联盟成立于2001年8月。2002年下半年，英国Invensys公司、日本三菱电气公司、美国摩托罗拉公司以及荷兰飞利浦半导体公司共同宣布加入ZigBee联盟，研发名为“ZigBee”的下一代无线通信标准，这一事件成为该技术发展过程中的里程碑。ZigBee联盟现有的理事公司包括BM Group，Ember公司，飞思卡尔半导体，Honeywell，三菱电机，摩托罗拉，飞利浦，三星电子，西门子，及德州仪器。ZigBee联盟的目的是为了在全球统一标准上实现简单可靠、价格低廉、功耗低、无线连接的监测和控制产品进行合作，并于2004年12月发布了第一个正式标准。

## 缩写与用语解释

- **AF** - Application Framework（应用层框架）。
- **APL** - Application Layer（应用层）。
- **APS** - Application Support sublayer（应用支撑层）。
- **MAC** - Medium Access Control layer（媒体访问控制层）。
- **NIB** - Network Information Base（网络信息库）
- **NWK** - Network layer（网络层）。
- **PHY** - Physical layer（物理层）。
- **WPAN** - Wireless Personal Area Network。为IEEE 802.15族系所规范的一系列无线个人区网标准。
- **ZC** - ZigBee Coordinator（ZigBee协调员）。
- **ZDO** - ZigBee Device Object（ZigBee设备对象）。
- **ZED** - ZigBee End Device（ZigBee终端设备）。
- **ZR** - ZigBee Router（ZigBee路由）。
- **FFD** - Full Function Device（全功能器件）。
- **RFD** - Reduce Function Device（精简功能器件）。

## 协议层与标准说明

ZigBee协议层从下到上分别为物理层（**PHY**）、媒体访问层（**MAC**）、网络层（**NWK**）、应用层（**APL**）等。网络设备的角色可分为 *ZigBee Coordinator、ZigBee Router、ZigBee End Device* 等三种。支持网络拓扑有星型、树型、网型等三种。

## 版本

*ZigBee V1.0*
这是第一个ZigBee标准公开版，于2005年6月开放下载，文件内记载公布时间为June 27, 2005，内部文件编号为053474r06。
*ZigBee V1.1*
第二个ZigBee标准公开版，于2007年1月开放下载，文件内记载公布时间为December 1, 2006，内部文件编号为053474r13。又称为ZigBee 2006。
*ZigBee V1.2*
第三个ZigBee标准公开版，于2008年1月开放下载，文件内记载公布时间为January 17, 2008，内部文件编号为053474r17。又称为ZigBee Pro、ZigBee 2007。

## 整理

### 信息库（Information Base）
ZigBee某些层有信息库存储该层所需信息，共有以下几种：

- MAC信息库（MIB）
- NWK信息库（NIB）
- APS信息库（AIB）

### Profile
ZigBee所定义的Profile有两种：

- Application Pro：针对各种不同应用情境所定义出的概略行为蓝图，如Home Control Lighting (HCL)和Home Automation (HA)。一般所称的Profile通常是指此种Profile。
- Stack Pro：主要规定通用性的网络参数，如Network Specific、Home Controls (HC)、Building Automation (BA)、Plant Control等Stack Profile。原则上Application Profile中会说明可采用何种Stack Profile来作为基础网络建构方案，如HCL中即采用HC作为网络建构方案。

### 各层定址

- **MAC**：可采用64位IEEE地址或16位NWK地址。
- **NWK**：16位NWK地址。
- **APS**：8位Endpoint号码。

>[参考链接](https://zh.wikipedia.org/wiki/ZigBee)
