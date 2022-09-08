# http2 - http2客户端

> 本页文档由[这个文件](https://gitee.com/openLuat/LuatOS/tree/master/luat/../components/network/libhttp/luat_lib_http.c)自动生成。如有错误，请提交issue或帮忙修改后pr，谢谢！

> 本库有专属demo，[点此链接查看http2的demo例子](https://gitee.com/openLuat/LuatOS/tree/master/demo/network)

## http2.request(method,url,headers,body,opts,ca_file)

http2客户端

**参数**

|传入值类型|解释|
|-|-|
|string|请求方法, 支持 GET/POST|
|string|url地址|
|tabal|请求头 可选 例如{["Content-Type"] = "application/x-www-form-urlencoded"}|
|string|body 可选|
|tabal|额外配置 可选 包含dst:下载路径,可选 adapter:选择使用网卡,可选|
|string|证书 可选|

**返回值**

|返回值类型|解释|
|-|-|
|int|code|
|tabal|headers |
|string|body|

**例子**

```lua
local code, headers, body = http2.request("GET","http://site0.cn/api/httptest/simple/time").wait()
log.info("http2.get", code, headers, body)

```

---
