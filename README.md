# vue-webpack-cube for hbuilder

> 此项目设计的最初目的是为了解决使用 vue+webpack 自动化构建并实时同步手机热更新调试而诞生。截止目前，DCloud 官方并提供一套完整的 vue+webpack+hbuilder 实时开发调试的文章，只是零零散散有人去构建一些自己的项目，并不能很好地教会或者引导大量开发者使用该开发模式进行开发。本项目以构建流程为主，适量 demo 为辅，印证了 vue+webpack+hbuilder 实时调试以及打包的可行性，为开发者提供多开发种选择。</br>
本APP与其他APP不同，该APP并不是功能性APP，所以几乎没有展示内容的业务逻辑，你可以把它理解为DCLOUD的muiAPP，做UIdemo的展示，并且验证PLUS在vue+webpack构建方式下的各类使用情况。更多的AQ可以在APP中的‘ABOUT’中得到解答。</br>
本应用为多页面开发，单页面请参照我的另一个APP：[vue-webpack-mint-for-hbuilder](https://github.com/wjsljc/vue-webpack-mint-for-hbuilder "vue-webpack-mint-for-hbuilder")

## 使用步骤
###下载代码
```
$ git clone https://github.com/wjsljc/vue-webpack-cube-for-hbuilder.git
$ cd vue-webpack-cube-for-hbuilder
$ npm install
```

### 在浏览器中调试调试
```
$ npm run dev
```
浏览器地址为：``http://localhost:8080/html/index.html``

### 真机同步调试
```
$ npm run dev
```
在 HBuilder 中设置应用入口地址为 ``本地服务器:端口号/html/index.html``
如 192.168.11.102:8080/html/index.html
> 请确保手机与本地服务在同一网段，否则无法访问本机的服务。

### 编译后真机同步调试
```
$ npm run build
```
- 把 dist 目录下的文件复制到 HBuilder 项目下
- 设置起始页为 html/index.html
- 真机运行调试

## 主要架构以及特色
> vue + webpack + cube-ui + hbuilder
- UI模块和PLUS模块独立展示，参考使用各取所需
- UI是对cube-ui官网demo的仿造与实际实践，采用的是后编译，100%迁移以及额外的扩展，更多的自定义demo展示与结合APP的运用，更加符合一款APP的基础需求
- PLUS对5+SDK的的集成运用，对APP常用的几个功能进行了展示，验证5+在vue中的使用
- 索引页面、登陆与登出，登陆超时、广告弹出等等功能的基础实现原理，使得APP更加“高仿”
- 对公共函数的封装、组件的封装、对公用代码mixin的使用等也体现了作者对APP的态度

## 赞助
如果该项目给您带来了工作上的参考或者启发，亦或者期待更多其他项目的诞生和该项目的继续维护，支持作者原创扫一扫或点击识别下方的二维码，为作者打赏1.0元吧！

![avatar](http://chuantu.biz/t6/319/1527238314x-1404795840.png)
![avatar](http://chuantu.biz/t6/319/1527238392x-1404793017.png)

