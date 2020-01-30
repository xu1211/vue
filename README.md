# vue
 vue学习

## 后端中的 MVC 与 前端中的 MVVM关系
 + MVC 是后端的分层开发概念；
 View视图层 --> Controller层 --> Model层
 + MVVM是前端视图层的概念，主要关注于 ==视图层分离== ，也就是说：MVVM把后端View视图层，又分为了 三部分 Model, View , VM ViewModel

Model(每个页面单独的数据) <--> VM ViewModel <--> View(每个页面的HTML)

最后就变成了:
后端V (前端M <--> 前端VM <--> 前端V) --> 后端C --> 后端M

1. [vue基础](/01.Vue的MVVM分层.html)
2. [常用指令](/02.常用指令.html)
3. [事件修饰符](/03.事件修饰符.html)
4. [双向绑定](/04.v-model双向绑定.html)
5. []()