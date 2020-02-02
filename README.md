# vue
 vue学习
## Vue调试工具`vue-devtools`的安装步骤和使用

[Vue.js devtools - 翻墙安装方式 - 推荐](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd?hl=zh-CN)

## 后端中的 MVC 与 前端中的 MVVM关系
 + MVC 是后端的分层开发概念；
 View视图层 --> Controller层 --> Model层
 + MVVM是前端视图层的概念，主要关注于 ==视图层分离== ，也就是说：MVVM把后端View视图层，又分为了 三部分 Model, View , VM ViewModel

Model(每个页面单独的数据) <--> VM ViewModel <--> View(每个页面的HTML)

最后就变成了:
后端V (前端M <--> 前端VM <--> 前端V) --> 后端C --> 后端M

1. [vue基础](/01.Vue的MVVM分层.html)
2. [指令](/02.常用指令.html)
3. [事件修饰符](/03.事件修饰符.html)
4. [双向绑定](/04.v-model双向绑定.html)
5. [外联样式](/05.vue中样式-class.html)
6. [内联样式](/06.vue中样式-style.html)
7. [v-for](/07.v-for循环.html)
8. [v-for中key属性的使用](/08.v-for循环中key属性的使用.html)
9. [渲染控制](/09.v-if和v-show的使用.html)
10.[过滤器](/10.过滤器的基本使用.html)
11.[按键修饰符](/11.按键修饰符.html)
12.[自定义指令]