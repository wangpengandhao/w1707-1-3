谈一谈你对渐进增强和优雅迭代的理解？

渐进增强

优雅降级



vue	编程思想

mvc

model内容、view如何去呈现内容、controller把内容放到视图里面

vue 生命周期 		钩子函数



1、创建对象

2、要将试图获取到

3、数据和视图绑定


## vue 双向数据绑定的重要原理     react  脏值绑定


```

Object.defineProperty(obj,"name",{

get(){
	return name
}
set(){
  
}

})
```
```
虚拟dom
前端工程化   开启者
angular

react   学习曲线    陡峭   无指令
vue  学习曲线  平缓
指令 过滤器  组件化
1、当做具有特殊功能的 属性
2、vue 提供的一种弥补html缺陷的一种方式
3、发展方向
```

###对象是类的事例，类是对象的抽象

## 组件化开发  
angular  react  vue

开发理念

解决html+css最需要组件化开发的语言，没有组件化

为了程序和功能的复用

提高开发效率  降低代码维护成本

### 完善的组件
结构	逻辑	数据
###　全局组件：
```
Vue.component("custom",{
       props:["con"],
       template:`<div @click="change">{{name}}</div>`,
       data(){
           return {
               name:this.con
           }
       },
       methods:{
           change(){
               this.name="lisi";
           }
       }
   })
```
v-bind:  动态数据绑定

单向数据流：方向：外层->里层

vue  外层的数据不能访问里层

双向数据绑定

### 局部组件
```
components:{
    custom:{
         props:["con"],
         template:`<div @click="change">{{name}}</div>`,
         data(){
             return {
                 name:this.con
             }
         },
         methods:{
             change(){
                 this.name="lisi";
             }
         }
     }
}
```
```
前端  mvc  c并不明确
    能够前后台分离- 分工明确-  维护成本低
    后台  mvc m（数据） v（html） c（php）
    路由：前台的路由
    确定 请求和组件之间的关系
    单页面的应用 SPA

    多页面  服务器 -> 相应 ->新的页面
    1、接收用户的请求
    2、分析用户的请求
    3、根据请求要获取相应的资源
    4、对资源来进行解析
    5、解析完成以后返回服务器
    6、返回个客户端

    Vue
    1、接收用户的请求
    2、分析用户的请求
    3、找到用户的数据
    4、返回给浏览器
    闭包有什么优略势？
    js内存泄露
    跨域
    vue-router  基本原理
    ajax 跨域 jsonp  代理（跨域）
```

```
即能用户体验友好，又能够对爬虫友好，又能够记录当前访问的标识  #one（锚链接）
http://[用户名:密码]@www.baidu.com/a/b?id=10#one
```

```
锚链接访问本地的请求，不发生跳转
/del/:id
post req.params.id
/del
get req.query.id
```

## 2018、01、03

```
能够让基于b/s架构的软件 像c/s架构的软件易于的操作*/
php 主流 优秀 简单
在js中分号和换行是耦合的
在php里面分号和换行不耦合
```

```
vue 编程式的导航
this.$route  当前导航的信息
this.$router  当前路由的信息
res.redirect("/add")  跳到add页面
```

```
嵌套路由
* router嵌套关系和component嵌套关系一一对应
* router-link里的部分参数
* event exact tag active-class
```

