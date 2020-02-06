# vue
 vue学习

## 后端中的 MVC 与 前端中的 MVVM关系
 + MVC 是后端的分层开发概念；
 View视图层 --> Controller层 --> Model层
 + MVVM是前端视图层的概念，主要关注于 ==视图层分离== ，也就是说：MVVM把后端View视图层，又分为了 三部分 Model, View , VM ViewModel

Model(每个页面单独的数据) <--> VM ViewModel <--> View(每个页面的HTML)

最后就变成了:
后端V (前端M <--> 前端VM <--> 前端V) --> 后端C --> 后端M

## 使用方法:
1. 网页开发直接通过script导入，会自动安装
<script src="/path/to/vue-router.js"></script>

2. NMP 模块化工程中使用它，必须要通过 Vue.use() 明确地安装路由功能
npm install vue-router
```
import Vue from 'vue'
```
## Vue调试工具`vue-devtools`的安装步骤和使用

[Vue.js devtools - 翻墙安装方式 - 推荐](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd?hl=zh-CN)

1. [vue基础](/01.Vue的MVVM分层.html)
el,date属性
2. [指令与方法](/02.常用指令.html)
methods属性
3. [事件修饰符](/03.事件修饰符.html)
4. [双向绑定](/04.v-model双向绑定.html)
v-model指令
5. [外联样式](/05.vue中样式-class.html)
6. [内联样式](/06.vue中样式-style.html)
7. [v-for](/07.v-for循环.html)
8. [v-for中key属性的使用](/08.v-for循环中key属性的使用.html)
9. [渲染控制](/09.v-if和v-show的使用.html)
v-if和v-show指令
10. [过滤器](/10.过滤器的基本使用.html)
filters属性
11. [按键修饰符](/11.按键修饰符.html)
12. [自定义指令](/12.自定义指令.html)
directive方法,directives属性
13. [>>生命周期](/生命周期.md)
8个会在固定时机执行的方法
14. [用三方包vue-resource发送http请求](/14.vue-resource基本使用.html)
15. [>>组件](/组件.md)
16. [ref获取dom元素和组件](/20.ref获取DOM元素和组件.html)
17. [>>路由](/路由.md)
18. [watch监听属性](/26.watch.html)
watch属性
19. [案例:watch监听非DOM元素](/27.watch-监视路由地址的改变.html)
20. [computed计算属性](/28.computed.html)
computed属性


## `data`、`watch`、`computed`和`methods`之间的对比
1. `data`: 定义属性, 属性值变化都会反馈在页面上
2. `watch`: 定义function，键是需要监听的表达式，值是对应回调函数 不需要return值。在键值改变后调用回调函数;
3. `computed`: 定义function, 需要return一个值, 所依赖的 响应式属性 有变化就会重新计算, 结果会被缓存，主要把键当作属性来使用；
4. `methods`: 主要书写业务逻辑, 可以使用`methods` 来替代 `computed`，效果上两个都是一样的，但是 computed 是基于它的依赖缓存，只有相关依赖发生改变时才会重新取值。而使用 methods ，在重新渲染的时候，函数总会重新调用执行。

