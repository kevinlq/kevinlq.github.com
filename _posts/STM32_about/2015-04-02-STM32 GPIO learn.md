---
layout : post
title: STM32中GPIO的8种模式理解
category : STM32学习
wangyiyun: true
date : 2015-04-02
---

******

    作者:鹅卵石
    时间:2015年04月02日21:14:16
    版本:V 0.0.0
    邮箱:kevinlq@yeah.net

<!-- more -->

# STM32中GPIO的8种模式理解

## 浮空模式
顾名思义就是浮在空中，上面用绳子一拉就上去了，下面用绳子一拉就沉下去了

## 开漏模式

就等于输出口接了个NPN三极管，并且只接了E，B，而C极是开	 	路的，你可以接一个电阻到3.3V，也可以接一个电阻到5V，这	样，在输出1的时候，就可以是5V电压，也可以是3.3V电压了，	但是不接电阻上拉的时候，这个输出高就不能实现了

## 推挽模式

就是有推有拉，任何时候IO口的电平都是确定的，不需要外接	上拉或者下拉电阻