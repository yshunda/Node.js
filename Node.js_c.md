> title Node.js学习笔记(三)Node.js核心模块之http模块
> date: 2017-1-08 19:08:24

## Node.js核心模块之http模块
> Http模块主要用于搭建http服务,使用Node.js搭建HTTP服务器非常简单.
* 服务器对象(创建一个服务器.监听计算机上的指定端口)
    - `let server=http.creatServer(fn)`
    - fn(请求 响应)
* 客户端对象(通过Node写一个客户端向服务端发送请求)
* 请求对象 请求体的数据获取."信息"
    * 包含信息
        - 获取请求首行中的url `request.url`
        - 获取头信息对象 `request.headers` -> {}
        - 获取请求方式 `request.method`
    * 在一次请求中，如何区分用户的行为含义呢
        - 结合url来判断，并且也会加上method来区分
* 响应对象 "功能"