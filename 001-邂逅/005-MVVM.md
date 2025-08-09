状态一变，自动 或 手动 调用 API 让界面更新，叫 数据驱动界面渲染

如果界面改变，对应绑定状态一并同步更新，叫 界面驱动状态更新，这往往出现在表单元素中

如果同时实现了 数据驱动界面渲染，又实现了 界面驱动状态更新，就叫 双向驱动视图更新「 双向绑定 」



React 只实现了 数据驱动界面渲染，而Vue默认实现了双向绑定



为了实现 数据驱动界面渲染或双向绑定，有两种架构模式

1. MVC 「 Model – View –Controller 」 => 实现关注点分离：模型、视图、控制器，并在此基础上实现了数据驱动视图重新渲染
2. MVVM 「 Model-View-ViewModel 」 => 在MVC 的基础上实现了双向数据绑定



React只规定了如何描述UI，并不规定代码组织方式，但其可以看成是类MVC框架

Vue 受MVVM启发，开发过程中参考了MVVM框架，虽然没有完全遵循MVVM架构，但依旧可以将Vue看成是类MVVM框架



![image.png](https://s2.loli.net/2025/08/09/FrHJ4ydqesITlmw.png) 

Vue 在 MVVM 架构中 充当 VM的角色，只要完成

+ Data Bindings 将 状态自动绑定到界面上
+ DOM Listeners 自动监听界面用户交互，并触发并执行对应事件回调