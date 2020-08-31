# SPMOD - BT


## 概述

<img src="../../assets/spmod/sipeed_spmod_bt.jpg" alt="XXX" style="zoom:60%;" />

SPMOD-BT(BLE 模块)采用 YDJ-23。

## SPMOD - BLE 介绍

- 采用 **Sipeed-SPMOD** 接口(2.54mm * 8PIN 排针)，统一 MaixPy 开发板接口
- 利用 SP-MOD UART 和蓝牙模块通讯
- JDY-23蓝牙模块：支持BLE 5.0（兼容 BLE4.0、BLE4.2）。具有UART接口。模块支持AT指令控制。具备超低功耗特性和高可靠性
- 板载两个状态指示LED，模块状态一目了然
- 模块尺寸：25.6\*20.2\*3.2mm

### JDY-23 蓝牙介绍


| 功能特点： | 参数 |
| --- | -- |
| 工作频段：| 2.4G |
| 发射功率：| 4db（最大） |
| 通信接口：| UART |
| 工作电压：| 1.8V~3.6V |
| 工作温度：| -40℃ - 80℃ |
| 天线：| 板载PCB天线 |
| 接收灵敏度：| -97dbm |
| 主从支持：| 从机 |
| 蓝牙版本：| BLE 5.0（兼容 BLE4.0、BLE4.2） |
| 唤醒状态电流：| 800uA（广播模式） |
| 浅睡状态电流：| <50uA (广播模式) |
| 深度睡眠电流：| 9uA （无广播） |
| 默认串口波特率：| 9600 |


- 主要 AT 指令列表

| 指令 | 描述 |
| --- | --- |
|AT+POWR | 显示模块发送功率 |
|AT+RST	| 软复位 |
|AT+MAC	| 显示MAC 地址 |
|AT+NAME | 显示广播名 |
|AT+HOSTEN | 从模式或 IBEACON 工作模式 |
|AT+IBUUID | IBEACON 的 UUID |
|AT+DISC | 指令断开连接 |
|AT+SLEEP | 睡眠 |
|AT+MTU | 设置模块发送的发包数长 |

> 详细的 AT 指令列表以及用法，请参考 JDY-23 AT 指令说明


###  SPMOD_XXX 模块引脚定义：


| 引脚序号  | 引脚名称 | 类型  | 引脚说明    |
| -------- | -------- | ---- | ---------- |
| 1        | GND      | G    | 模块电源地  |
| 2        | AWK      | I/O  | NOTE: |
| 3        | STA      | I/O  | 连接状态引脚，蓝牙已连接，输出高电平，未连接低电平 |
| 4        | RX       | I    | 串口接收引脚|
| 5        | TX       | O    | 串口发送引脚|
| 6        | RST      | I/O  | 复位引脚，低电平有效 |
| 7        | ---      | NC   |            |
| 8        | VCC      | V    | 模块电源    |

## 使用例程

- MaixPy 例程：

> NOTE: 待更新

- STM32 例程：

> NOTE: 待更新

## 参考设计


- SPMOD_XXX 原理图：

-----

## 资源链接

| 资源 | --- |
| --- | --- |
| 官网 | www.sipeed.com |
| SIPEED 官方淘宝店 |[sipeed.taobao.com](sipeed.taobao.com) |
|Github | [https://github.com/sipeed](https://github.com/sipeed) |
|BBS | [http://bbs.sipeed.com](http://bbs.sipeed.com) |
|MaixPy 文档官网 | [http://maixpy.sipeed.com](http://maixpy.sipeed.com) |
|Sipeed 模型平台 | [https://maixhub.com](https://maixhub.com) |
|SDK 相关信息 | [https://dl.sipeed.com/MAIX/SDK](https://dl.sipeed.com/MAIX/SDK) |
|HDK 相关信息 | [https://dl.sipeed.com/MAIX/HDK](https://dl.sipeed.com/MAIX/HDK) |
|E-mail(技术支持和商业合作) | [Support@sipeed.com](mailto:support@sipeed.com) |
|telgram link | https://t.me/sipeed ||MaixPy AI QQ 交流群 | 878189804 |
|MaixPy AI QQ 交流群(二群) | 1129095405 |
