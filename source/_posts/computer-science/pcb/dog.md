---
title: 《开源pcb-四足机器狗》
date: 2020/06/13 20:56:48
categories:
- [PCB,开源设计,原理图,硬件设计]
tags:
- PCB
- 开源设计
- 原理图
- 开源
valine:
  placeholder: "1. 提问前请先仔细阅读本文档⚡\n2. 页面显示问题💥，请提供控制台截图📸或者您的测试网址\n3. 其他任何报错💣，请提供详细描述和截图📸，祝食用愉快💪"
audio:
  - https://music.163.com/song?id=1387098940
password: 123
---

https://tva4.sinaimg.cn/large/007n4kghly8h73pe98jz1j30u00k0q5x.jpg


# 项目介绍：<span class="colour" style="color:#0000000">设计一款四足机器人，样子如下</span>

![frount2.18.jpg](//image.lceda.cn/pullimage/DtoVyNRLxR3bBQr5NtObPNjsW9qjqx25ZtK3Apt3.jpeg)
![untitled.14.jpg](//image.lceda.cn/pullimage/vHykDEkr7mvvEJfwgBxS2DWOC4yK21nzyv1sg4Sf.jpeg)
![Keyshot_Animation.gif](//image.lceda.cn/pullimage/QtMwjgX0kWagRxXnUMsmQTv0yp8e2jCwMrZEY19E.gif)

# B站视频链接：

# 版本1：<span class="colour" style="color:rgb(255, 0, 255)">（刚出生就癫痫的bilibili）18650电池供电</span>[https://www.bilibili.com/video/BV1ra411M7d1](https://www.bilibili.com/video/BV1ra411M7d1)

# 版本2：<span class="colour" style="color:rgb(255, 0, 255)">（更换狗粮之后，癫痫治好了）更换航模电池</span>[https://www.bilibili.com/video/BV1mt4y1G7aC](https://www.bilibili.com/video/BV1mt4y1G7aC)

# 实际上3D打印回来组装完成是这样：

![微信图片_202207140048149.jpg](//image.lceda.cn/pullimage/hZglajFiJHHtpwlUVL0vWS0MYz6BDmoHtujYjLgk.jpeg)
![微信图片_202207140048144.jpg](//image.lceda.cn/pullimage/GWOEjudOZHB752oqg9B0QnQ3CUHe53A7emuUJxjR.jpeg)
![微信图片_202207140048146.jpg](//image.lceda.cn/pullimage/t2CQWvUSYg0lV4EhaqrMOcIRv9B4Ljds1XPBqrrY.jpeg)

# 行动展示

![123333 \(1\).gif](//image.lceda.cn/pullimage/yHDxRVF0NMwdygKN79UvmDS5eQhlBlX48dk6u8Q2.gif)
![GIFFFF \(2\).gif](//image.lceda.cn/pullimage/JgHK2DSEieo3ZenyspoAO3K5VQw4KYrI1Qc2UA3d.gif)

# 项目分析：

## 一、<span class="font" style="font-family:方正粗黑宋简体">结构部分</span>

### 参考灯哥四足机器人结构制作，附件为最新版的3D图纸，可直接打样生产，生产价格为200元左右。 具体开源链接点击这里：[灯哥开源四足机器人项目](https://github.com/ToanTech/py-apple-quadruped-robot) ![3D打印费用.png](//image.lceda.cn/pullimage/PgCINBVFDbrMWBNGd49PW5JQdHijEqrW1KqK5Xnm.png)

## 二、电路部分

### 1、基于鸿蒙Hi3861主控，支持鸿蒙系统开发。[采购链接](https://item.szlcsc.com/3235616.html)

### 2、8路舵机采用驱动芯片PCA9685PW来管理，此芯片可控制多达16路的舵机。采用IIC接口与单片机连接。

### 3、MPU6050模块通过读取角速度，陀螺仪数据来识别狗狗当前的状态，从而更好的控制狗狗行走。

## 三、软件部分

### 1、采用鸿蒙开发平台进行开发，开发环境为ubuntu20 Linux环境编译，windows平台串口烧录程序

## 四、组装部分

### 1、配件采购：

#### （1）大腿连接轴承：<span class="colour" style="color:rgb(0, 0, 255)"></span>

需要采购4pcs。[采购链接](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.423c2e8dc6Gw9v&id=669696763433&_u=ee1q309e152)![微信截图_20220714011633.png](//image.lceda.cn/pullimage/UXRWupR5r0fGxxDodwZUwTw3tIc1727LZIB5a5hr.png)

#### （2）防松螺母：连接必须要购买防松螺母，不然走几步就松了。<span class="colour" style="color:rgb(0, 0, 255)"></span>

采购M2 M3型号各10pcs。

[采购链接](https://detail.tmall.com/item.htm?id=17861747572&spm=a1z09.2.0.0.423c2e8dc6Gw9v&_u=ee1q3093d38&skuId=4915326594693)![微信截图_20220714011825.png](//image.lceda.cn/pullimage/w5YFw6gKmvwy6yP0ChWdLg4xbqpLqX2IZV7AbGtX.png)

#### （3）小腿拉杆总成：<span class="colour" style="color:rgb(0, 0, 255)"></span>

采购M2X35mm 4pcs [采购链接](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.423c2e8dc6Gw9v&id=628756983115&_u=ee1q309ce1d)<br>
<br>
![微信截图_20220714012252.png](//image.lceda.cn/pullimage/2rZSpj7tkC0kgO6xfuicXWLWo8nFsyTXQGrPOoEV.png)

#### （4）MG90S舵机：<span class="colour" style="color:rgb(0, 0, 255)"></span>

采购8pcs [采购链接](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.423c2e8dc6Gw9v&id=19375870769&_u=ee1q3090dfa)<br>
<br>
![微信截图_20220714012553.png](//image.lceda.cn/pullimage/TuXVobWbWhsSdd8D3T1aprXhvBTZ5GGPN1twaQh4.png)

#### （5）MPU6050模块：<span class="colour" style="color:rgb(0, 0, 255)"></span>

采购1pcs [采购链接](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.423c2e8dc6Gw9v&id=16630417522&_u=ee1q3093744)<br>
<br>
![微信截图_20220714012816.png](//image.lceda.cn/pullimage/xKfgO9TWY3bnMRRuseZ9QO9z6T1P9pxwNBlSXFZs.png)

#### （6）螺丝：[采购链接](https://detail.tmall.com/item.htm?id=600221526381&spm=a1z09.2.0.0.423c2e8dc6Gw9v&_u=ee1q30953c3)

| 螺丝名称 | 采购数量 |
| ---- | ---- |
| m2X8自攻螺丝 | 10pcs |
| m2*10自攻螺丝 | 10pcs |
| m2*10细牙螺丝 | 10pcs |
| m2*15细牙螺丝 | 10pcs |
| m3*25细牙螺丝 | 10pcs |
| m3*10细牙螺丝 | 10pcs |

![微信截图_20220714013011.png](//image.lceda.cn/pullimage/BSj85R9kgtxDbRrioWjQqP4pxxCk9kN98wdwOUPV.png)

#### （7）电池：[采购链接](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.37462e8dCHnCTO&id=552179995972&_u=je1q309a027)

![微信截图_20220719162931.png](//image.lceda.cn/pullimage/iBaFGNYHz683CIawfbHcexiM9yENOpWNTV2bVInS.png)

#### （8）遥控器：可不买 WIFI控制它不香么[采购链接](https://item.taobao.com/item.htm?spm=2013.1.20160405.13.612449daznmjFJ&scm=1007.13066.167449.0&id=561245318271)

![微信截图_20220714151059.png](//image.lceda.cn/pullimage/Bl9nHwEfCRHT0uf77bKANri50m294Mt6eylsSihC.png)

## 原理图设计说明

### <span class="colour" style="color:rgb(255, 0, 255)">锂电池充电，放电，升压电路</span>

![微信截图_20220714013820.png](//image.lceda.cn/pullimage/hTNcC7admnosshcWGPRrQCJxLy5M61AQ0296FHOd.png)

## PCB设计说明

![微信截图_20220714013918.png](//image.lceda.cn/pullimage/3wcQ1TcdPfEl8Z18PbbxFb1a5Qz22jf2FDr93oo0.png)

## 软件说明

# 狗狗运动算法简述： [参考菠萝狗](http://padog.com.cn/#/PAD-3.0-Manual/5%E7%90%86%E8%AE%BA%E8%A7%92/5.1%E5%85%AB%E8%87%AA%E7%94%B1%E5%BA%A6/%E5%85%AB%E8%87%AA%E7%94%B1%E5%BA%A6)

### 算法参考：灯哥四足机器人 [【教程】灯哥0基础DIY四足机器人指南](https://www.bilibili.com/video/BV1b5411L7ks?p=17)

## 一、运动学正解

* 已知：大腿、小腿的角度
* 求：足端坐标

### 1、运动学正解解算过程

机器狗的腿部按图中的位置放置，在腿部所在平面作一个坐标系，如下图所示。大腿和x轴形成的夹角为A1（大腿的角度），大腿延长线和小腿形成的夹角为A2 （小腿的角度）。
![微信截图_20220714101437.png](//image.lceda.cn/pullimage/1TyAicRFVZJRzmnugdOM0gwd3hq8PfIKeutq6vF3.png)
![theory_8degree_forwardKinematics_1.png](//image.lceda.cn/pullimage/MH6r71dMcNLu83nq9Gl34cG5lfpsJOsODMjhXCT6.png)

### 2、计算方法

![微信截图_20220714101645.png](//image.lceda.cn/pullimage/fJCQbYQgfcVCPnB3kxHIRgGVSpJPv6WOYYTEgzwe.png)

### 3、旋转变换--参考灯哥开源视频：[旋转变换](https://www.bilibili.com/video/BV1Hp4y1D7zn?zw&vd_source=ce835e443ac546d1988d810ee9a6f6cb)

## 二、运动学逆解

* 已知：足端坐标
* 求：大腿、小腿的角度
![1.png](//image.lceda.cn/pullimage/m59hJwpHoizd95Y4pA30oRggWQLBPmzjnfmjOOKm.png)
![2.png](//image.lceda.cn/pullimage/aI98A8GiPXEiGi0fsAAfqi8NYdHu8uj2B9Nel1zf.png)![3.png](//image.lceda.cn/pullimage/DMqrn225BmiXuR2JipQWZnGq9NhkSj2U1ma6ghDw.png)

## 实物展示说明

![2022_07_19_12_42_IMG_5983.JPG](//image.lceda.cn/pullimage/ftt86iRwGfN889g72SQ1gMFd77e6ZwYXWPEOh0vV.jpeg)!
![2022_07_19_12_43_IMG_5986.JPG](//image.lceda.cn/pullimage/wVZmGDdW1HJIyHEJeKUY9ZZpJHsQNe4Kg9hJ3WkG.jpeg)
![微信图片_202207140048142.jpg](//image.lceda.cn/pullimage/38zPqdBiUQ0fLyjaodLqvUg08O6l4e8muDT0cKr4.jpeg)

## 问题未解决

### ~~1、电路板设计V2.0版本，目前版本因为电流过大，只能使用数据线供电，18650电池带不动8个舵机，瞬间电流在2A左右。~~

![微信图片_20220719163239.jpg](//image.lceda.cn/pullimage/uCVJ53vENRsXOdRmUShxaSFpAtmuMb9M6u7V4Oxv.jpeg)

### <span class="colour" style="color:rgb(0, 255, 0)">7月22日已经解决，更换供电部分，采用航模电池供电</span>

![微信图片_20220722155929.jpg](//image.lceda.cn/pullimage/vTccEv5ujSPkUmdaP9mDwrU7ZNwwm7xz26q6pKgo.jpeg)

### 2、添加mpu6050模块作为狗的姿态验证，软件编写中，未完成

### 3、计划添加K210模块作为狗的脑袋摄像头，作为物品识别，物体跟踪，有计划，还未实施。

### 4、电路板整合起来，现在为各种电路板拼接。

## 演示视频