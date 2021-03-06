一个基于Nodejs koa2的博客;
使用了ejs渲染模板，目前只有首页;
这个blog目前只是个基本雏形，完善中 ^_^！


Folder structure
=====

```
.
├── bin                         #启动脚本 node ./bin/www
├── config                      #config
├── demo                        #demo
├── log                         #操作日志
├── middlewares                 #自定义中间件
├── models                      #model层
├── public                      #静态资源
├── routes                      #路由层
├── schema                      #schema层
├── services                    #业务层
├── test                        #单元测试
├── utils                       #工具类
└── views                       #视图层

```
初步截图
=====

### pc端
![blog_pc](./public/images/blog_pc.png)

详情页
![topic_detail](./public/images/topic_detail.png)

### 移动端
![blog_pc](./public/images/blog_mobile.png)

Features
=====
* 支持markdown
* comment评论            //TODO
* message board留言板    //TODO
* 支持async/await 函数 (Babel required)
* node.js v7.6.0+
* 启动 npm start
* mongoose mongodb ORM module

Install
=====
    1. git clone https://github.com/mosaic101/koa2-blog.git
    2. cd koa2-blog
    3. npm install
    4. npm start
    5. http://localhost:4000
    <!--6. 需要本地安装redis，并启动-->

Notice
=====
    1. 依赖node.js v7.6.0+ (Koa requires node v7.6.0 or higher for ES2015 and async function support.)
    2. koa-session 依赖包是基于cookie的,已经好久不维护了。这里用 koa-generic-session
    3. async/await 函数是es7的特性,async函数里使用await可以做到和yield类似的效果，但await只能接promise对象
    4. 用bluebird替换原生Promise,blurbird的性能是V8里内置的Promise 3倍左右bluebird 的优化方式见 https://github.com/petkaantonov/bluebird/wiki/Optimization-killers ）。

Ps
=====
    1. 觉得有帮助的顺手给颗星，十分谢谢！
    2. 欢迎大家提宝贵意见！
