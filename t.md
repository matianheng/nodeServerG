
# 2.制作后端 node 服务器
#初始化项目

#新建文件夹, 起名为 node-server , 新建文件 app.js , 在终端中初始化项目
 
 npm init
 npm i

# 我们想要制作服务器, 这里使用 express 来实现

1
npm i --save express
# 当然了, 我们还需要解决跨域问题, 这里使用 cors 来解决

1
npm i --save cors
# 现在我们来考虑前端传参问题
# 对于get请求，其参数是直接拼接在url后面的，解析也相对容易。在express框架中，get请求的参数全部都被放置在了request对象的query中。
# post请求有多种形式可以发送数据，这取决于post请求的请求头Content-type的内容，常见的有三种：

# multipart/form-data
# application/x-www-form-urlencoded
# application/json
# 为此，我们引入中间件来解决读取参数的问题
# 这里使用 body-parser 和 connect-multiparty 来解决

1
npm i --save body-parser
1
npm i --save connect-multiparty


// 1
// npm i --save cors

# 启动命令
node app.js
# 安装 mysql 依赖

1
npm i --save mysql

# 前后端交互我们使用 axios
# 安装依赖

1
npm i --save axios

# 访问地址 http://127.0.0.1:3000/getStudent
