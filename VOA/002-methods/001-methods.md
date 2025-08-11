1. 语法格式为 `Record<方法名，函数>`
2. 方法内部 `this` 指向暴露的代理对象
   + 所以不推荐将方法定义为箭头函数
3. methods 中的属性和方法可以在组件初始化时被挂载到代理对象上
   + 可以直接在模板中使用
   + 可以直接通过代理对象访问



<iframe
  src="https://stackblitz.com/github/coder-klaus/vue3-tutorial/tree/learn/voa?file=src%2F002-methods%2F001-%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8.html&view=editor"
  width="100%"
  height="600"
  origin="https://github.com/coder-klaus/vue3-tutorial/blob/learn/voa/src/002-methods/001-%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8.html"
  frameborder="0"
  allowfullscreen
></iframe>

