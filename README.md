# Data-Visualization-Web
一个数据可视化大屏的vue2、vue3、react项目集合

- [lofTV-Screen](https://gitee.com/daidaibg/IofTV-Screen#https://gitee.com/link?target=https%3A%2F%2Fwww.daidaibg.com%2Fbigscreen)

  预览地址：https://www.daidaibg.com/bigscreen/#/index

  Vue2+JS+Axios+Echarts+Element-ui+vuex  有屏幕自适应

- [lofTV-Screen-Vue3](https://gitee.com/daidaibg/IofTV-Screen-Vue3#https://gitee.com/link?target=https%3A%2F%2Fwww.daidaibg.com%2Fbigscreen-vue3)

  预览地址：https://www.daidaibg.com/bigscreen-vue3/#/index

  Vue3+TS+Axios+Echarts+Element-plus+vuex  有屏幕自适应

>注意：vue2需要vetur插件，vue3需要volar插件并禁用veturl
>
>node：vue2用14即可，vue3现在我用的是18

- [vue-big-screen](https://gitee.com/MTrun/big-screen-vue-datav)

  Vue2+Echarts+vuex   数据写死在vue的data中  有屏幕自适应

- [vue-big-screen-plugin](https://gitee.com/MTrun/vue-big-screen-plugin#https://gitee.com/MTrun/big-screen-vue-datav)

  Vue3+TS+vuex  数据写死在tsx中

> 注意：vue3的我没有跑起来

- [react-big-screen](https://gitee.com/MTrun/react-big-screen)

  React+JS+fetch  有屏幕宽度自适应，高度需要滚动

  mock数据   调用util/request.js   所有接口在service/index.js暴露

> 注意：React这个真的好看

---------

### 1.Fetch、Axios、Ajax

- Ajax

  xhr.readyState：

  - 0：刚创建的XMLHttpRequest实例
  - 1：（载入）已调用send()，正在发送请求
  - 2：（载入完成）send()方法执行完成，已经接收到全部的响应数据
  - 3：loading(交互)正在解析响应内容
  - 4：done解析完成

  从TCP上来说，get产生一个TCP数据包；Post产生两个（先发header服务器响应100continue，再发data服务器响应200）

- Axios

  一个基于**Promise**的现代化HTTP客户端，是目前最流行的 HTTP 客户端，可以在浏览器和Node.js环境中发送HTTP请求，并具有拦截请求（`axios.interceptors.request`）和响应（`axios.interceptors.response`）、支持并发请求、提供丰富的API等功能。

  使用Promise封装的Ajax

- Fetch

  不是Ajax，而是原生的JS

  基于Promise实现

> 白嫖一下 看看苏琪翔的图解TCP

### 2.框架演进（原生JS、JQuery、Vue2、Vue3、React、Angular）

- JQuery淘汰了原生JS

  因为JQuery可以快速选取对象，方便操作DOM。

  原生JS去操作Ajax时，要从新建XMLHttpRequest对象开始；JQuery从`$.ajax`开始

- Vue淘汰了JQuery

  操作DOM是一个极其浪费性能的方式，Vue取代JQuery最根本的原因是**数据的双向绑定**

  axios的出现

> Vue2与Vue3区别，为什么会出现Vue3

- 双向数据绑定原理不同
- Vue2不支持碎片；Vue3支持碎片，可以拥有多个根节点
- 定义数据变量和方法不同
- 生命周期钩子函数不同

### 3.vue-cli与vite区别

vue-cli是vue2使用的

vite是vue3使用的

