https-server
============= 
<html>
<body>
<h3> Basic https server that can host a simple web page.</h3>
<h3>Server:</h3>
<pre class="prettyprint lang-js">
var http = require('http');

http.createServer(function (request, response) {

    // 发送 HTTP 头部 
    // HTTP 状态值: 200 : OK
    // 内容类型: text/plain
    response.writeHead(200, {'Content-Type': 'text/plain'});

    // 发送响应数据 "Hello World"
    response.end('Hello World\n');
}).listen(8080);

// 终端打印如下信息
console.log('Server running at http://127.0.0.1:8080/');
</pre>
</body>
</html> 
