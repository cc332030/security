
# HSTS 严格传输安全协议
（HTTP Strict Transport Security）

## 问题
假设网站已设置访问 HTTP 时重定向到 HTTPS，黑客可以拦截 HTTP 请求防止进行 HTTPS 浏览器，并展开后续攻击

## 作用
强制客户端（如浏览器）使用HTTPS与服务器创建连接，即使黑客拦截了替换 HTTPS 为 HTTP，浏览器依旧使用 HTTPS 方式

