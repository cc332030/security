
# MIME类型混淆攻击 X-Content-Type-Options

通过设置"X-Content-Type-Options: nosniff"响应标头，对 script 和 styleSheet 在执行是通过MIME 类型来过滤掉不安全的文件。

- 如果通过 styleSheet 参考检索到的响应中接收到 "nosniff" 指令，则 Windows Internet Explorer 不会加载“stylesheet”文件，除非 MIME 类型匹配 "text/css"。

- 如果通过 script 参考检索到的响应中接收到 "nosniff" 指令，则 Internet Explorer 不会加载“script”文件，除非 MIME 类型匹配以下值之一：
    - application/ecmascript
    - application/javascript
    - application/x-javascript
    - text/ecmascript
    - text/javascript
    - text/jscript
    - text/x-javascript
    - text/vbs
    - text/vbscript

[https://blog.51cto.com/volvo9yue/1903432](https://blog.51cto.com/volvo9yue/1903432)
