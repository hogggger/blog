1.最近遇到一个需求，有一个父组件
```javascript
<father></father>
和两个子组件
<child1></child1>
<child2></child2>
```
子组件都需要向父组件请求一个数据，有两种方法获取这个数据，第一种是父组件请求数据，然后再把数据传给子组件；
第二种方法是子组件各自请求数据；朋友给了几个参考标准：看子组件是业务组件还是通用组件；看接口的支持情况（回传数据的使用范围）
一开始我选择的是通过父组件在挂载的时候请求数据,是用钩子mounted(){};但是