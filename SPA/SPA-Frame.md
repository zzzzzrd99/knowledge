# SPA框架
## 为什么选择使用框架而不是原生[参考](https://juejin.im/post/5d5f44dae51d4561df7805b4)
* 组件化
* 天然分层 代码解耦
* 生态链完整
* 开发效率
## 虚拟 DOM 的优缺点
* 虚拟DOM
* 优点
    * 保证性能下限：通过diff，找出最小差异，然后批量进行patch
    * 无需手动操作DOM：虚拟DOM的diff和parch都是在一次更新中自动进行的
    * 跨平台：虚拟DOM本质上是javascript对象，而DOM与平台强相关
* 缺点
    * 无法进行极致性优化：在一些性能要求极高的应用中虚拟DOM无法进行针对性的极致优化,
## 虚拟 DOM 实现原理
## 什么是 MVVM
> 由数据驱动，实现数据的双向绑定
* Model 数据模型
* View UI组件
* ViewModel 同步View 和 Model的对象
## 说说你对 SPA 单页面的理解，它的优缺点分别是什么
> 就是在 Web 页面初始化时加载所有的 HTML、JavaScript 和 CSS，页面的内容的变化，靠动态创建dom
* 优点
    * 用户体验好、快，内容的改变不需要重新加载整个页面，避免了不必要的跳转和重复渲染；
    * 基于上面一点，SPA 对服务器的压力小；
    * 前后端职责分离，架构清晰，前端进行交互逻辑，后端负责数据处理；
* 缺点
    * 初次加载耗时多，为实现单页 Web 应用功能及显示效果，需要在加载页面的时候将 JavaScript、CSS 统一加载，部分页面按需加载；
    * 前进后退路由管理，由于单页应用在一个页面中显示所有的内容，所以不能使用浏览器的前进后退功能，所有的页面切换需要自己建立堆栈管理
    * SEO 难度较大，由于所有的内容都在一个页面中动态替换显示，所以在 SEO 上其有着天然的弱势