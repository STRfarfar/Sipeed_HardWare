# SPMOD - Weather


## 概述

<img src="../../assets/spmod/sipeed_spmod_weather.jpg" alt="SPMOD - Weather" style="zoom:60%;" />

SPMOD - Weather (气象站模块), 集成三轴传感器 QMC7983,与温湿度气压传感器 BME280。


## SPMOD - Weather 介绍

特性：

- 采用 **Sipeed-SPMOD** 接口(2*4PIN 2.54mm 排针)，统一 MaixPy 开发板接口
- 通过SP-MOD I2C接口连接
- 磁性传感器：QMC7983是一个内置灵敏度补偿与NTC的三轴磁性传感器，I2C接 输出（最高频率400KHz），具有出色的动态范围和精度以及超低的功耗
- 磁感应量程：±30 高斯
- 温湿度气压传感器：BME280是同时集成了温湿度与气压传感器的数字传感器
- 模块尺寸：25.0\*XX.X\*XX.Xmm


## 传感器特性：

|磁性传感器：| QMC7983 |
| --- | --- |
| 工作电压：| 2.6V~3.6V |
| 工作电流：| 70uA |
| 休眠电流：| <1uA |
| 磁感应量程：| ±30 高斯 |
| 精度：| 每 LSB 1mG|
| RMS 噪声：| 2 mG |
| 对外接口： |I2C，默认地址 0x2C,可通过选择电阻调节 |


| 温湿度气压传感器： | BME280 |
| --- | --- |
| 工作电压： | 1.71V~3.6V |
| 工作电流： | <633uA |
| 休眠电流： | <5uA |
| 湿度传感器的关键参数： | |
| | 响应时间（𝜏63％）1 s |
| | 精度公差 ±3％ 相对湿度 |
| | 磁滞 ±1％ 相对湿度 |
| 气压力传感器的关键参数： |
| | RMS 噪声 0.2 Pa，等效 到海拔 1.7 厘米 |
| | 偏移温度系数 ±1.5 Pa/K，等效温度变化 1°C 时达到海拔 ±12.6 cm1s |
| 对外接口： |I2C，默认地址 0x76, 可通过选择电阻调节 |

###  SPMOD_XXX 模块引脚定义：


| 引脚序号 | 引脚名称 | 类型 | 引脚说明      |
| -------- | -------- | ---- | ------------- |
| 1        | GND      | G    | 模块电源地    |
| 2        | ---      | NC   |               |
| 3        | ---      | NC   |               |
| 4        | SDA      | I/O  | I2C 数据线    |
| 5        | SCL      | I    | I2C 时钟线    |
| 6        | ---      | NC   |               |
| 7        | ---      | NC   |               |
| 8        | VCC      | V    | 模块电源 3.3V |

> I/O 表示信号输入/输出(以模块视角)
>
> V/G 表示电源 VCC/GND
>
> NC 表示该引脚无电气连接

## 使用例程

- MaixPy 例程：

> NOTE: 待更新

- STM32 例程：

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
