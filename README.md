### peter老师课程

#### 第一节
* http://haoduoshipin.com
* happypeter.github.io/js-tiger/
* es6/react/JS/H5/ 技术动手开发Web应用的能力
### 具体的点
* es6
* react基础
* Redux
* 项目实战
#### 什么是Node.js/nvm?
* nodejs 是 js 的运行环境。
#### 什么是es6？
* es 是 Javascript 的背后的标准名。es6 是Js 的新标准，目前提到es6指的是‘新JS’
* ES6 的功能，浏览器只能大部分支持，开发时，用到ES6，一定涉及到’编译’的概念，准确的说是‘转译’，把es6转换为老js语法，保证浏览器可以支持。
* #### ES6 是新的JS 的语法的总和
* #### 如何转译es6？
* 使用Babel来转译。http://babeljs.io 可以试用，  但是实际开发中都是在命令行中自动化的使用babel
* create-react-app 这个开发环境集成了babel


## 面向对象编程
* class 关键字是es6的新特性，定义‘类’
* constructor 构造函数 对象被创建的时候， 自动被呼叫的一个方法
`
  class Person{
    constructor(){
      console.log(1)
    }
    say(){
      console.log(2)
    }
    let lj = new Person;
  }
`
### 如何使用类的继承？
* `
class Person{
  sayWords(){
    console.log('I am humen')
  }
}
class women extends Person{
  sayMe(){
    console.log('I am king')
  }
}
let i= 0
let mm = new women
mm.sayMe()
mm.sayWords()
`
* 首先要有父类Person，再写子类：class 子类名 extends 父类名{}
* extends 本意“拓展”，这里‘继承’

* 子类的constructor中用到this会报错，要添加super()解决


#### es6 Module(模块)
* 模块默认隔离所有内容
* 隔离：如果在模块中声明一个变量或函数，默认其他文件（模块）中无法访问.
* ##### 导出的两种形式：
* 默认导出:export default Person,对应的导入方式：import Person from ‘./Person’。一个模块只能导出一次并且只导出一个变量。
* 命名导出：export{Person,i},对应的导入方式：import{Person，i} from ./Person
* import/export 是es6的新关键字，普通浏览器包括nodejs都还不支持，所以要到create-react-app环境中运行

### let const
* var 的缺陷：
  问题多：作用域不清晰；可以重复声明，代码有错误，不容易报错出来；
  * let const 避免了var的缺陷
  * let 声明变量；后续允许修改
  * const 声明常量,一旦修改就会报错
#### 解构赋值是什么？
* 是后续开发中常用的一种赋值方式，特点：简短易懂,并没有新功能。被认为是一种语法糖。

#### 模板字符串
* 倒引号（波浪号的键）  ${变量名}
* `let name = 'lj'；
let str = `my name is ${name}`；
console.log(str)
`

#### 箭头函数
* 使函数更为简短，同时省去绑定this的麻烦
原来的函数写成
* `const myFun = function(name){
  console.log(name)
}
`
* 现在的函数写成
* `const myFun = (name) =>{
  console.log(name)
}
myFun('lj')
`
* 如果参数只有一个，那么可以把参数括号去掉，写成

* `const myFun = name =>{
  console.log(name)
}
`
* 同时如果里面只有一条，那么花括号也可以省去。
* `const myFun = name =>console.log(name)
`
* 如果希望输出两倍name
* `const myFun = name =>{
  return name +name
}
console.log(myFun('lg'))
`
* 但是箭头函数有一个好处，默认就是返回最后的值，所以可以写成
* `const myFun = name => name + name
`
