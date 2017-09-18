### peter3
* 全局css基本可以不用，type-face除外（中文网站很少用）
组件名骆驼。对应的css名小写，中划线隔开
state 中存放react组件内部会变化的数据  只读性
this.handleClick 事件响应函数
handleClick可以看成变量
.setState

this.state.statName
render 里面都是标签代码，render重新执行，类似手动刷新，但是整个页面不会刷新，刷新的只是当前组件
事件：.onClick,
.onSubmit 只用于表单提交
&&  运算符，表示逻辑与（and），当运算符两边的表达式的结果都为true时，整个运算结果才为true，否则，只要有一方为false，则结果为false。
&& 还具有短路的功能，即如果第一个表达式为false，则不再计算第二个表达式，
### peter 5
* jsx 中插入数组不加key就会报错“数组中的每个子元素都需要一个独特的key”。加key的目的：便于区分各个元素
× map里箭头函数的后面的小括号是return的内容（箭头函数的简写形式），用小括号圈成一个整体
* 如何向事件处理函数中传递参数：在外层包裹一个无名函数
* onClick={()=>this.change2(i)}
###### 判断的两种写法
× className={this.state.activeIndex===i ? 'active':''}
× className={this.state.activeIndex1===i && 'active'}
