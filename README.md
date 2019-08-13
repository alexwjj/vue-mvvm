# mvvm

一个简单的mvvm的实现，参考**Vue**中的模板编译、数据绑定和`render`函数的生成。

不用安装任何依赖，直接`npm start`， 然后访问[http://127.0.0.1:8888](http://127.0.0.1:8888)即可查看效果。

**src**文件夹中是具体`mvvm`的实现，主要有三个文件：

* **mvvm.js**是框架入口文件，其中包括了调用`oberser`监听对象，根据`ast`生成`render`函数，并执行`render`函数生成最终的`dom`内容。
*  **observe.js**中，就是对`data`数据进行监听。
*  **parse**中，是把传入的`template`字符串解析为一个`ast`，供生成`render`时候使用。