# string - 额外添加了一些字符串操作函数

> 本页文档由[这个文件](https://gitee.com/openLuat/LuatOS/tree/master/luat/../lua/src/lstrlib.c)自动生成。如有错误，请提交issue或帮忙修改后pr，谢谢！

## string.toHex(str)

将字符串转成HEX

**参数**

|传入值类型|解释|
|-|-|
|string|需要转换的字符串|

**返回值**

|返回值类型|解释|
|-|-|
|string|HEX字符串|
|number|HEX字符串的长度|

**例子**

```lua
string.toHex("\1\2\3") --> "010203" 3
string.toHex("123abc") --> "313233616263" 6
string.toHex("123abc"," ") --> "31 32 33 61 62 63 " 6

```

---

## string.fromHex(hex)

将HEX转成字符串

**参数**

|传入值类型|解释|
|-|-|
|string|hex,16进制组成的串|

**返回值**

|返回值类型|解释|
|-|-|
|string|字符串|

**例子**

```lua
string.fromHex("010203")       -->  "\1\2\3"
string.fromHex("313233616263") -->  "123abc"

```

---

## string.split(str, delimiter)

按照指定分隔符分割字符串

**参数**

|传入值类型|解释|
|-|-|
|string|输入字符串|
|string|分隔符|

**返回值**

|返回值类型|解释|
|-|-|
|table|分割后的字符串表|

**例子**

```lua
("123,456,789"):split(',') --> {'123','456','789'}

```

---

## string.toValue(str)

返回字符串tonumber的转义字符串(用来支持超过31位整数的转换)

**参数**

|传入值类型|解释|
|-|-|
|string|输入字符串|

**返回值**

|返回值类型|解释|
|-|-|
|string|转换后的二进制字符串|
|number|转换了多少个字符|

**例子**

```lua
string.toValue("123456") --> "\1\2\3\4\5\6"  6
string.toValue("123abc") --> "\1\2\3\a\b\c"  6

```

---

## string.urlEncode("123 abc")

将字符串进行url编码转换

**参数**

|传入值类型|解释|
|-|-|
|string|需要转换的字符串|

**返回值**

无

**例子**

无

---

## string.toBase64(str)

将字符串进行base64编码

**参数**

|传入值类型|解释|
|-|-|
|string|需要转换的字符串|

**返回值**

|返回值类型|解释|
|-|-|
|string|解码后的字符串,如果解码失败会返回空字符串|

**例子**

无

---

## string.fromBase64(str)

将字符串进行base64解码

**参数**

|传入值类型|解释|
|-|-|
|string|需要转换的字符串|

**返回值**

|返回值类型|解释|
|-|-|
|string|解码后的字符串,如果解码失败会返回空字符串|

**例子**

无

---
