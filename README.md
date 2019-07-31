# mvvm_example
本实例通过实现以下 4 个步骤，来实现数据的双向绑定：

1、实现一个监听器 `Observer` ，用来劫持并监听所有属性，如果属性发生变化，就通知订阅者；

2、实现一个订阅器 `Dep`，用来收集订阅者，对监听器 `Observer` 和 订阅者 `Watcher` 进行统一管理；

3、实现一个订阅者 `Watcher`，可以收到属性的变化通知并执行相应的方法，从而更新视图；

4、实现一个解析器 `Compile`，可以解析每个节点的相关指令，对模板数据和订阅器进行初始化。‘

相关结构图表示如下：

![3.png](https://github.com/fengshi123/blog/blob/master/assets/mvvm/3.png?raw=true) 

## 构建步骤

1、需要 Node.js 6+ （作者使用的版本为：node.js 8.2.1 npm 5.3.0）

2、如果你需要更改 js 代码，比如说打些 console.log 查看运行的结果等，需要进行 js 编译压缩，步骤如下：

- 安装插件：npm install

- 运行示例：npm run build

- 然后会生成 js 压缩文件，放在目录 /dist 下面

3、运行示例，可以用浏览器打开 /example/index.html 运行示例页面。

4、实例展示如下：

![1.gif](https://github.com/fengshi123/blog/blob/master/assets/mvvm/1.gif?raw=true) 