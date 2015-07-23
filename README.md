# React基本学习及示例

## jsx语法写代码

## 用React些组件component
* this.props
* this.state
* React.findDOMNode
* this.props.children

##  form表单
* DOM事件

## state状态机
	* getInitialState
	* this.state && this.setState
## 组件生命周期

> 组件的生命周期分成三个状态,React为每个状态都提供了两种处理函数，will 函数在进入状态之前调用，did函数在进入状态之后调用，三种状态共计五种处理函数。

* Mounting：已插入真实 DOM
	* componentWillMount()
	* componentDidMount()
* Updating：正在被重新渲染
	* componentWillUpdate(object nextProps, object nextState)
	* componentDidUpdate(object prevProps, object prevState)
* Unmounting：已移出真实 DOM
	* componentWillUnmount()

> 两种特殊状态的处理函数

* componentWillReceiveProps(object nextProps)
	* 已加载组件收到新的参数时调用
* shouldComponentUpdate(object nextProps, object nextState)
	* 组件判断是否重新渲染时调用