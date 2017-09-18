## peter老师课程之2
* 数组es6新方法 .find()  .map() .filter() .reverse()
* 对象方法 Object.assign(目标对象，合并对象，合并对象....) 复制合并对象,目标对象也会改变
```js
let obj1={a:1}
let obj2={
  b:1,
  c:2
}
let obj3={d:6}
let obj4 = Object.assign(obj1,obj2,obj3)
console.log(obj4)
console.log(obj1)
let obj1={a:1}
let obj2={
  b:1,
  c:2
}
let obj3={d:6}
let obj4 = Object.assign(obj1,obj2,obj3)
console.log(obj4)
console.log(obj1)
```
* Object.keys()  可以把一个对象的所有的key(属性名)都拿出来，组成一个数组。再把新的数组用数组（.map()）方法处理。比for... in方法更适合做对象迭代
* 展开运算符  ...  三个点
* promise 在JS中是一个盒子，其中包含一个将要被完成的事件。
* 编程风格：目前最流行的JS编程风格，一种是AirBnb，另外一种是标准编程风格（推荐使用）。
* 标准编程风格特点：不写分号

###新建nodejs项目
* 新建文件夹,命令行npm init -y 生成json文件，npm install 包名
### create-react-app
* 开发react项目的环境，无需配置直接使用
* 若安装失败后，先运行npm config set registry
http://registry.npm.taobao.org
* yarn.lock 类似npm
* public 文件夹放html和图标
* src文件夹 放所有的js
* npm start开始运行react
* index.html,文件基本是空的，用来挂在react组件
* App.js  是react的组件
* index.js 主要使用reactDom这个包,作用是把react组件挂到index.html中唯一的一个div
动手写react组件：1，导入必要的变量`import React,{Component} from 'react'``
jsx：react 项目组自己发明的一种文件格式。在js中使用类似html
不能用class，而要用className
