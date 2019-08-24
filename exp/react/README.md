<!-- TOC -->

- [React Context API使用方法](#react-context-api%e4%bd%bf%e7%94%a8%e6%96%b9%e6%b3%95)
- [React高阶组件](#react%e9%ab%98%e9%98%b6%e7%bb%84%e4%bb%b6)
- [React监听DOM改变](#react%e7%9b%91%e5%90%acdom%e6%94%b9%e5%8f%98)
- [React循环输出方法](#react%e5%be%aa%e7%8e%af%e8%be%93%e5%87%ba%e6%96%b9%e6%b3%95)
- [React生命周期](#react%e7%94%9f%e5%91%bd%e5%91%a8%e6%9c%9f)
- [React设置默认props参数](#react%e8%ae%be%e7%bd%ae%e9%bb%98%e8%ae%a4props%e5%8f%82%e6%95%b0)
- [React获取状态参数](#react%e8%8e%b7%e5%8f%96%e7%8a%b6%e6%80%81%e5%8f%82%e6%95%b0)
- [React绑定事件方法](#react%e7%bb%91%e5%ae%9a%e4%ba%8b%e4%bb%b6%e6%96%b9%e6%b3%95)
- [React路由渲染方式](#react%e8%b7%af%e7%94%b1%e6%b8%b2%e6%9f%93%e6%96%b9%e5%bc%8f)

<!-- /TOC -->

## React Context API使用方法

实现按钮中英文之间的切换

```js
import ReactDOM from 'react-dom';
import Hoc from "./views/context.jsx";

ReactDOM.render(
    <Hoc />,
    document.querySelector('#root')
);
```

context.jsx

```js
import React from "react";

const enStrings = {
    submit: "Submit",
    cancel: "Cancel"
}

const cnStrings = {
    submit: "提交",
    cancel: "取消"
}

const LocaleContext = React.createContext(enStrings);

class LocaleProvider extends React.Component{
    state = {locale: cnStrings};
    toggleLocale = () => {
        const locale = this.state.locale === enStrings ? cnStrings : enStrings;
        this.setState({locale});
    };
    render() {
        return (
            <LocaleContext.Provider value={this.state.locale}>
                <button onClick={this.toggleLocale}>切换语言</button>
                {this.props.children}
            </LocaleContext.Provider>
        )
    }
}

class LocaleButtons extends React.Component{
    render() {
        return (
            <LocaleContext.Consumer>
                {locale => (
                    <div>
                        <button>{locale.cancel}</button>&nbsp;<button>{locale.submit}</button>
                    </div>
                )}
            </LocaleContext.Consumer>
        )
    }
}

export default () => (
    <div>
        <LocaleProvider>
            <div>
                <br />
                <LocaleButtons />
            </div>
        </LocaleProvider>
    </div>
)
```


## React高阶组件

```js
import ReactDOM from 'react-dom';
import Hoc from "./views/hoc.jsx";

ReactDOM.render(
    <Hoc />,
    document.querySelector('#root')
);
```

app.jsx

在这里高阶组件withTimer只负责传参不进行组件UI设置

```js
import React from "react";

// 高阶组件
function withTimer(WrappedComponent){
    return class extends React.Component {
        state = {time: new Date()};
        componentDidMount(){
            this.timerID = setInterval(() => this.tick(), 1000);
        }
        componentWillUnmount(){
            clearInterval(this.timerID);
        }
        tick(){
            this.setState({
                time: new Date()
            });
        }
        render(){
            return <WrappedComponent time={this.state.time}{...this.props} />
        }
    }
}

class App extends React.Component {
    render() {
        return (
            <div id="home-container">
                <p>现在时间是：</p>
                <p>{this.props.time.toLocaleString()}</p>
            </div>
        );
    }
}

export default withTimer(App);
```

## React监听DOM改变

```js
import React from 'react';
import ReactDOM from 'react-dom';

function ForList(props){
    const numbers = props.value;
    const listItems = numbers.map((number,index) =>
        <li key={number.toString()}>{number}/{index}</li>
    );
    return (
        <ul>{listItems}</ul>
    );
}

class App extends React.Component {
    constructor(props) {
        super(props);
        this.state = {
            listItem: []
        }
    }
    // 监听改变前DOM
    getSnapshotBeforeUpdate(){
        return this.rootNode.innerHTML;
    }
    // 监听改变前DOM
    componentDidUpdate(perProps, perState, domHtml) {
        // 改变前DOM结构
        console.log(domHtml);
        // 改变后DOM结构
        console.log(this.rootNode.innerHTML);
    }
    componentDidMount() {
        console.log(3);
        this.timerId = setInterval(() => this.addListData(),1000);
    }
    addListData(){
        this.setState(pre => ({
            listItem: [new Date().getTime(), ...pre.listItem],
        }))
    }
    render(){
        return (
            <div ref={node => (this.rootNode = node)}>
                <ForList value={this.listItem} />
            </div>
        )
    }
}

ReactDOM.render(
    <App />,
    document.querySelector('#root')
);
```

## React循环输出方法

```js
import React from 'react';
import ReactDOM from 'react-dom';

function ForList(props){
    const numbers = props.value;
    const listItems = numbers.map((number,index) =>
        <li key={number.toString()}>{number}/{index}</li>
    );
    return (
        <ul>{listItems}</ul>
    );
}

class App extends React.Component {
    constructor(props) {
        super(props);
        this.state = {
            listItem: [1,2,3,4,5,6]
        }
    }
    render(){
        return (
            <div>
                <ForList value={this.listItem} />
            </div>
        )
    }
}

ReactDOM.render(
    <App />,
    document.querySelector('#root')
);
```

## React生命周期

```js
import React from 'react';
import ReactDOM from 'react-dom';

class App extends React.Component {
    constructor(props) {
        super(props);
    }
    // 1.DOM渲染前方法
    componentWillMount(){
        console.log(1)
    }
    // 2.DOM渲染
    render(){
        return (
            <div></div>
        )
    }
    // 3.DOM渲染后方法
    componentDidMount() {
        console.log(3);
    }
}

ReactDOM.render(
    <App />,
    document.querySelector('#root')
);
```

## React设置默认props参数

```js
import React from 'react';
import ReactDOM from 'react-dom';

class App extends React.Component {
    constructor(props) {
        super(props);
    }
    render(){
        // 输出Colin
        return (
            <div id="main">
                {this.props.name}
            </div>
        )
    }
}
// props是不可变更的内容
App.defaultProps = {
    name: 'Colin'
};

ReactDOM.render(
    <App />,
    document.querySelector('#root')
);
```

## React获取状态参数

```js
import React from 'react';
import ReactDOM from 'react-dom';

class App extends React.Component {
    constructor(props) {
        super(props);
        // 状态数据管理
        this.state = {
            title: 'This is title'
        };
    }
    render(){
        return (
            <div id="main">
                {this.state.title}
            </div>
        )
    }
}

ReactDOM.render(
    <App />,
    document.querySelector('#root')
);
```

## React绑定事件方法

```js
import React from 'react';
import ReactDOM from 'react-dom';

// 第一种方法
// handleClick()无法获取this必须使用.bind(this)绑定this

class App extends React.Component {
    constructor(props) {
        super(props);
        // 状态数据管理
        this.state = {
            isToggleOn: false
        };
    }
    // 添加点击事件
    handleClick() {
        this.setState(prevState => ({
            isToggleOn: !prevState.isToggleOn
        }));
    }
    render(){
        return (
            <div id="main">
                <button onClick={this.handleClick.bind(this)}>改变isToggleOn值</button>
            </div>
        )
    }
}

// 第二种方法
// 使用handleClick = () => {}方法可以保留this指向

class App extends React.Component {
    constructor(props) {
        super(props);
        // 状态数据管理
        this.state = {
            isToggleOn: false
        };
    }
    // 添加点击事件
    handleClick = () => {
        this.setState(prevState => ({
            isToggleOn: !prevState.isToggleOn
        }));
    }
    render(){
        return (
            <div id="main">
                <button onClick={this.handleClick}>改变isToggleOn值</button>
            </div>
        )
    }
}

// 第三种方法
// 在创建事件时使用(e) => this.handleClick(e)指向this

class App extends React.Component {
    constructor(props) {
        super(props);
        // 状态数据管理
        this.state = {
            isToggleOn: false
        };
    }
    // 添加点击事件
    handleClick() {
        this.setState(prevState => ({
            isToggleOn: !prevState.isToggleOn
        }));
    }
    render(){
        return (
            <div id="main">
                <button onClick={(e) => this.handleClick(e)}>改变isToggleOn值</button>
            </div>
        )
    }
}

ReactDOM.render(
    <App />,
    document.querySelector('#root')
);
```

## React路由渲染方式

```js
// React路由渲染分为BrowserRouter和HashRouter
import { BrowserRouter,HashRouter } from "react-router-dom";
import Root from './routes.js';

// BrowserRouter路由为history模式
ReactDOM.render(
    <BrowserRouter>
        <Root />
    </BrowserRouter>,
    document.querySelector('#root')
);

// HashRouter路由为纯前端#切换
ReactDOM.render(
    <HashRouter>
        <Root />
    </HashRouter>,
    document.querySelector('#root')
);
```

routes.js

```js
import React from 'react';
import { Route, Switch, Redirect } from 'react-router-dom';

import App from './../app.jsx';

import Home from './../views/home.jsx';
import about from './../views/about.jsx';

const Root = () => (
   <div>
      <Switch>
         <Route
            path="/"
            render={props => (
               <App>
                  <Switch>
                     <Route path="/" exact component={Home} />
                     <Route path="/home" component={Home} />
                     <Route path="/about" component={about} />
                      {/*路由不正确时，默认跳回home页面*/}
                     <Route render={() => <Redirect to="/" />} />
                  </Switch>
               </App>
            )}
         />
      </Switch>
   </div>
);

export default Root;
```