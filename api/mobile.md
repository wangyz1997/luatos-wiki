# mobile - 蜂窝网络

> 本页文档由[这个文件](https://gitee.com/openLuat/LuatOS/tree/master/luat/../components/mobile/luat_lib_mobile.c)自动生成。如有错误，请提交issue或帮忙修改后pr，谢谢！


## mobile.imei(index, newvalue)

获取或设置IMEI

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|
|string|新的IMEI. 不填就是获取IMEI, 填了就是设置IMEI, 是否支持设置取决于底层实现.|

**返回值**

|返回值类型|解释|
|-|-|
|string|当前的IMEI值|

**例子**

无

---

## mobile.imsi(index, newvalue)

获取或设置IMSI

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|
|string|新的IMSI. 不填就是获取IMSI, 填了就是设置IMSI, 是否支持设置取决于底层实现.|

**返回值**

|返回值类型|解释|
|-|-|
|string|当前的IMSI值|

**例子**

无

---

## mobile.apn(index, newvalue)

获取或设置APN

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|
|string|新的APN. 不填就是获取APN, 填了就是设置IMSI, 是否支持设置取决于底层实现.|

**返回值**

|返回值类型|解释|
|-|-|
|string|当前的APN值|

**例子**

无

---

## mobile.csq(index)

获取csq

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|

**返回值**

|返回值类型|解释|
|-|-|
|int|当前CSQ值|

**例子**

无

---

## mobile.rssi(index)

获取rssi

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|

**返回值**

|返回值类型|解释|
|-|-|
|int|当前rssi值|

**例子**

无

---

## mobile.rsrp(index)

获取rsrp

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|

**返回值**

|返回值类型|解释|
|-|-|
|int|当前rsrp值|

**例子**

无

---

## mobile.rsrq(index)

获取rsrq

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|

**返回值**

|返回值类型|解释|
|-|-|
|int|当前rsrq值|

**例子**

无

---

## mobile.snq(index)

获取snq

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|

**返回值**

|返回值类型|解释|
|-|-|
|int|当前snq值|

**例子**

无

---

## mobile.flymode(index, enable)

进出飞行模式

**参数**

|传入值类型|解释|
|-|-|
|int|编号,默认0. 在支持双卡的模块上才会出现0或1的情况|
|bool|是否设置为飞行模式,true为设置, false为退出|

**返回值**

|返回值类型|解释|
|-|-|
|bool|原飞行模式的状态|

**例子**

无

---
