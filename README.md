# Node.js服务器
## server-00.js文件
初版，获取各种路径
## server-01.js文件
这是一个简单的服务器配置文件<br>
实现以下功能<br>
1. 用户请求 / 时，返回 html 内容
2. 该 html 内容里面由一个 css link 和一个 script
3. css link 会请求 /style.css，返回 css 内容
4. script 会请求 /main.js，返回 js 内容
5. 请求 / /style.css /main.js 以外的路径，则一律返回 404 状态码
## server.js文件(后续可能会继续更新)
如果用户请求的路径是'/'的话，返回状态200，写入字符串'哈哈哈'，然后结束。
如果是其它的路径，那么返回404，并写入字符串'呜呜呜'，然后结束。
