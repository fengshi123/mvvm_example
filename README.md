# request_example
本实例实现了虚拟 DOM 的基础操作： 

 ● 用 `JS` 对象模拟 `DOM` 树 — `element.js`

 ● 比较两棵虚拟 `DOM` 树的差异 — `diff.js`

 ● 将两个虚拟 `DOM` 对象的差异应用到真正的 `DOM` 树 — `patch.js`

## 构建步骤

1、需要 Node.js 6+ （作者使用的版本为：node.js 8.2.1 npm 5.3.0）

2、如果你需要更改 js 代码，比如说打些 console.log 查看运行的结果等，需要进行 js 编译压缩，步骤如下：

- 安装插件：npm install

- 运行示例：npm run build

- 然后会生成 js 压缩文件，放在目录 /dist 下面

3、运行示例，可以用浏览器打开 /example/index.html 运行示例页面。