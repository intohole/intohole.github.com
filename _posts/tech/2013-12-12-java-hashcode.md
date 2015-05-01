---
layout: default
title: Java　Hashcode 
tags: [tech,java]
city: 南京
---


java hashcode 规则
==============================


|类型   |   散列码计算|
|--------------------------------------|:--------------------------------------------|
boolean | f ? 1 : 0
byte/char/short/int | (int)f
long | (int)(f^f(f>>>32))  
float | Float.floatToIntBits(f)  
double | Double.doubleToLongBits(f) ->(long)  
Arry | 每个元素按照上述操作，做，相加  



result = 31 * result + c ; //c 上述结果  
----------------------------------