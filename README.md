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
## server-02.js文件
使用jsonp发请求并给出响应。
1. 如果请求的路径是根路径的话，那么返回index-02.html。并且把index-02.html里 的字符串`&&&amount&&&`换成money.db文件中的字符串，也就是余额。
2. 在index-02.html中，如果点击打款按钮的话就会发送请求，请求的路径为"/pay"。服务器接收到请求后进行一个随机指定，如果随机数大于0.5的话返回200，执行回调函数提示打款成功，并把money.db文件中的值减去1。否则返回400。
## server.js文件(后续可能会继续更新)