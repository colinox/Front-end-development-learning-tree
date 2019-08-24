<!-- TOC -->

- [判断是否空对象](#判断是否空对象)
- [JavaScript获取屏幕分辨率（包含显示设置文本缩放）](#javascript获取屏幕分辨率包含显示设置文本缩放)
- [订阅者模式](#订阅者模式)
- [单例设计模式](#单例设计模式)
- [ES6合并对象方法](#es6合并对象方法)
- [类继承多个对象方法](#类继承多个对象方法)
- [判断是否类型错误](#判断是否类型错误)
- [手动实现bind、call、apply](#手动实现bindcallapply)
- [vue实现异步组件](#vue实现异步组件)
- [防抖动函数](#防抖动函数)
- [简单的节流函数](#简单的节流函数)
- [解构常用方法合集](#解构常用方法合集)
- [函数自执行方法](#函数自执行方法)
- [Object.create的基本实现原理](#objectcreate的基本实现原理)
- [JavaScript对象深拷贝](#javascript对象深拷贝)
- [使用filter和some快速筛选指定数据内容](#使用filter和some快速筛选指定数据内容)
- [使用索引或者映射实现switch语句](#使用索引或者映射实现switch语句)
- [使用some匹配部分条件](#使用some匹配部分条件)
- [every或find实现匹配所有条件](#every或find实现匹配所有条件)
- [includes实现多条件判断](#includes实现多条件判断)
- [instanceof实现原理](#instanceof实现原理)
- [JSON.stringify()替换输出内容](#jsonstringify替换输出内容)
- [最简单JS的去重方式 （重灾区）](#最简单js的去重方式-重灾区)
- [求最大值/最小值](#求最大值最小值)
- [高阶函数实现缓存(备忘模式)](#高阶函数实现缓存备忘模式)
- [优雅的向下取整](#优雅的向下取整)
- [JS 对象转 url 查询字符串](#js-对象转-url-查询字符串)
- [随机生成六位数字验证码](#随机生成六位数字验证码)
- [手动实现一个new方法](#手动实现一个new方法)
- [生成随机ID](#生成随机id)
- [生成随机十六进制代码（生成随机颜色）](#生成随机十六进制代码生成随机颜色)
- [ES7数组快速去重](#es7数组快速去重)
- [创建过去七天的数组](#创建过去七天的数组)
- [ES6快速处理URL地址参数](#es6快速处理url地址参数)
- [ES6快速合并对象内容并能相互替换](#es6快速合并对象内容并能相互替换)
- [ES6数组快速去重](#es6数组快速去重)
- [ES6函数参数设置默认空值返回错误](#es6函数参数设置默认空值返回错误)
- [实现两个字符串进行加法计算](#实现两个字符串进行加法计算)
- [实现两个字符串进行乘法计算](#实现两个字符串进行乘法计算)
- [两种简单的数组去重方案](#两种简单的数组去重方案)
- [获取选中内容并包裹标签更换内容](#获取选中内容并包裹标签更换内容)
- [深究setTime循环出现的问题](#深究settime循环出现的问题)
- [判断指定内容是否存在](#判断指定内容是否存在)
- [通过数组进行多条件并存判断](#通过数组进行多条件并存判断)
- [创建文本DOM方法](#创建文本dom方法)
- [字符串转数字快捷方法](#字符串转数字快捷方法)
- [向下取整快捷方法](#向下取整快捷方法)
- [柯里化正则验证写法](#柯里化正则验证写法)
- [函数传参转柯里化函数传参](#函数传参转柯里化函数传参)
- [ES6类的静态成员](#es6类的静态成员)
- [ES6类的继承](#es6类的继承)
- [继承内建对象](#继承内建对象)
- [继承表达式的类](#继承表达式的类)
- [只能继承的抽象类](#只能继承的抽象类)
- [ES6可计算的成员名称](#es6可计算的成员名称)
- [ES6访问器属性](#es6访问器属性)
- [原生js惯性滚动与回弹效果](#原生js惯性滚动与回弹效果)
- [中文和字母排序方法](#中文和字母排序方法)
- [DOM事件绑定方法](#dom事件绑定方法)
- [JS原生手写on和off绑定解绑方法](#js原生手写on和off绑定解绑方法)
- [阻止微信上拉底部回弹效果](#阻止微信上拉底部回弹效果)
- [监听页面属性或者结构发生变化触发](#监听页面属性或者结构发生变化触发)
- [&&在JS中的另类用途](#在js中的另类用途)
- [ECMA-262规范定义的七种错误类型](#ecma-262规范定义的七种错误类型)
- [强制触发JS错误提示并终止进程](#强制触发js错误提示并终止进程)
- [可编辑DIV的DIV标签改为P标签](#可编辑div的div标签改为p标签)
- [返回事件监听方法](#返回事件监听方法)
- [Range操作详解](#range操作详解)
- [过滤粘贴特殊标签](#过滤粘贴特殊标签)
- [光标处插入内容](#光标处插入内容)
- [捕获粘贴事件等操作方法](#捕获粘贴事件等操作方法)
- [横向滚动计算公式](#横向滚动计算公式)
- [手写简单的模板引擎](#手写简单的模板引擎)
- [js原生获取DOM元素在父元素内的下标值](#js原生获取dom元素在父元素内的下标值)
- [继承](#继承)
- [绑定this指向](#绑定this指向)
- [将类数组对象转换成数组对象](#将类数组对象转换成数组对象)
- [背景图实现多端大小适配](#背景图实现多端大小适配)
- [判断游览器是否支持touch事件](#判断游览器是否支持touch事件)
- [深入理解自定义事件绑定](#深入理解自定义事件绑定)
- [创建自定义事件并触发](#创建自定义事件并触发)
- [addEventListener绑定事件触发对象](#addeventlistener绑定事件触发对象)
- [instanceof原理](#instanceof原理)
- [||和&&的妙用](#和的妙用)
- [阻止touchstart点穿方法](#阻止touchstart点穿方法)
- [原生JS实现forEach代码](#原生js实现foreach代码)
- [随机指定范围数字](#随机指定范围数字)
- [前端计算分配随机概率](#前端计算分配随机概率)
- [JavaScript策略模式理解](#javascript策略模式理解)
- [window.location详细操作用法](#windowlocation详细操作用法)
- [手把手实现简单的模板数据渲染](#手把手实现简单的模板数据渲染)
- [深入拷贝对象方法](#深入拷贝对象方法)
- [JavaScript精准的类型判断](#javascript精准的类型判断)
- [数组去重的四种方法](#数组去重的四种方法)
- [JS原生实现extend方法](#js原生实现extend方法)
- [JS判断对象属性或方法是否属于原型链](#js判断对象属性或方法是否属于原型链)
- [深度优先遍历树结构](#深度优先遍历树结构)
- [数字千分位格式化](#数字千分位格式化)
- [二分查找](#二分查找)
- [获取元素距离页面的top、left](#获取元素距离页面的topleft)
- [JavaScript原生绑定事件和解绑事件](#javascript原生绑定事件和解绑事件)
- [回车触发事件](#回车触发事件)
- [对象深入拷贝方法](#对象深入拷贝方法)
- [JavaScript阻止事件动作](#javascript阻止事件动作)
- [JavaScript阻止冒泡和捕获](#javascript阻止冒泡和捕获)
- [call继承条件](#call继承条件)
- [createDocumentFragment()降低创建元素渲染次数](#createdocumentfragment降低创建元素渲染次数)
- [通过bind()掌控this](#通过bind掌控this)
- [把对象转JSON格式输出](#把对象转json格式输出)
- [判断是否为数组对象](#判断是否为数组对象)
- [JS判断显示页面是否为移动端](#js判断显示页面是否为移动端)
- [JS禁止滚轮、键盘触发滚动条滚动](#js禁止滚轮键盘触发滚动条滚动)
- [简单的前端路由机制](#简单的前端路由机制)
- [减少页面的重绘](#减少页面的重绘)
- [JS构建简单的路由系统](#js构建简单的路由系统)
- [Js/Jquery获取iframe中的元素](#jsjquery获取iframe中的元素)

<!-- /TOC -->

## 判断是否空对象

方法1：

ES6的新方法, 返回值也是对象中属性名组成的数组

```js
var data = {};
var arr = Object.keys(data);

console.log(arr.length === 0)  // true
```

方法2：

此方法是使用Object对象的getOwnPropertyNames方法，获取到对象中的属性名，存到一个数组中，返回数组对象，我们可以通过判断数组的length来判断此对象是否为空

> 注意：此方法不兼容ie8，其余浏览器没有测试

```js
var data = {};
var arr = Object.getOwnPropertyNames(data);

console.log(arr.length == 0); // true
```

方法3:

将json对象转化为json字符串，再判断该字符串是否为"{}"

```js
var data = {};
var b = (JSON.stringify(data) == "{}");

console.log(b);//true
```

## JavaScript获取屏幕分辨率（包含显示设置文本缩放）

```js
var xres = window.screen.width * window.devicePixelRatio
var yres = window.screen.height * window.devicePixelRatio

console.log("分辨率: " + xres + " X " + yres);
```

## 订阅者模式

```js
function Event() {
    this.handlers = {};
}
Event.prototype = {
    // 订阅事件
    on: function(eventType, handler) {
        var self = this;
        if (!(eventType in self.handlers)) {
            self.handlers[eventType] = [];
        }
        self.handlers[eventType].push(handler);
        return this;
    },
    // 触发事件(发布事件)
    emit: function(eventType) {
        var self = this;
        var handlerArgs = Array.prototype.slice.call(arguments, 1);
        for (var i = 0; i < self.handlers[eventType].length; i++) {
            self.handlers[eventType][i].apply(self, handlerArgs);
        }
        return self;
    },
    // 删除订阅事件
    off: function(eventType, handler) {
        var currentEvent = this.handlers[eventType];
        var len = 0;
        if (currentEvent) {
            len = currentEvent.length;
            for (var i = len - 1; i >= 0; i--) {
                if (currentEvent[i] === handler) {
                    currentEvent.splice(i, 1);
                }
            }
        }
        return this;
    }
};

let Publisher = new Event();
//订阅事件a
Publisher.on('a', function(e) {
    console.log(1 + e);
});
Publisher.on('a', function(e) {
    console.log(2 + e);
});

//触发事件a
Publisher.emit('a', '我是第1次调用');

Publisher.emit('a', '我是第2次调用');　
```


## 单例设计模式

```js
var Singleton = (function() {
    var instance;

    function createInstance() {
        var object = new Object("I am the instance");
        return object;
    }

    return {
        getInstance: function() {
            if (!instance) {
                instance = createInstance();
            }
            return instance;
        }
    };
})();

function run() {

    var instance1 = Singleton.getInstance();
    var instance2 = Singleton.getInstance();

    alert("Same instance? " + (instance1 === instance2));
}

run();
```

## ES6合并对象方法

```js
function createMenu(config) {
    config = Object.assign({
        title: "Foo",
        body: "Bar",
        buttonText: "Baz",
        cancellable: true
    }, config);
    // config now equals: {title: "Order", body: "Bar", buttonText: "Send", cancellable: true} // ...
}
```

## 类继承多个对象方法

```js
class Model {
    constructor() {}
}
class View {
    constructor() {}
}
class Controller {
    constructor(model, view) {
        this.model = model
        this.view = view
    }
}
const app = new Controller(new Model(), new View())
```

## 判断是否类型错误

```js
export default function add(a, b) {
    if (typeof (a) !== 'number' || typeof (b) !== 'number') {
        throw 'Error: parameters must be number.'
    }
    return a + b;
}
```

## 手动实现bind、call、apply

- call实现方法

```js
Function.prototype.call = function(content = window) {
    content.fn = this;
    let args = [...arguments].slice(1);
    let result = content.fn(...args);
    delete content.fn;
    return result;
}
let foo = {
    value: 1
}
function bar(name, age) {
    console.log(name)
    console.log(age)
    console.log(this.value);
}
bar.call2(foo, 'black', '18') // black 18 1
```

- apply实现方法

```js
Function.prototype.apply = function(context = window) {
    context.fn = this
    let result;
    // 判断是否有第二个参数
    if(arguments[1]) {
        result = context.fn(...arguments[1])
    } else {
        result = context.fn()
    }
    delete context.fn
    return result
}
```

- bind实现方法

会创建一个新函数。当这个新函数被调用时，bind() 的第一个参数将作为它运行时的 this，之后的一序列参数将会在传递的实参前传入作为它的参数。(来自于 MDN )

此外，bind实现需要考虑实例化后对原型链的影响。

```js
Function.prototype.bind = function(content) {
    if(typeof this != "function") {
        throw Error("not a function")
    }
    // 若没问参数类型则从这开始写
    let fn = this;
    let args = [...arguments].slice(1);

    let resFn = function() {
        return fn.apply(this instanceof resFn ? this : content,args.concat(...arguments) )
    }
    function tmp() {}
    tmp.prototype = this.prototype;
    resFn.prototype = new tmp();

    return resFn;
}
```

## vue实现异步组件

```js
const AsyncComponent = () => ({
    // 需要加载的组件 (应该是一个 `Promise` 对象)
    component: import('./MyComponent.vue'),
    // 异步组件加载时使用的组件
    loading: LoadingComponent,
    // 加载失败时使用的组件
    error: ErrorComponent,
    // 展示加载时组件的延时时间。默认值是 200 (毫秒)
    delay: 200,
    // 如果提供了超时时间且组件加载也超时了，
    // 则使用加载失败时使用的组件。默认值是：`Infinity`
    timeout: 3000
})
```

## 防抖动函数

```js
function debounce(fn, wait = 50, immediate) {
    let timer;
    return function () {
        if (immediate) {
            fn.apply(this, arguments)
        }
        if (timer) clearTimeout(timer)
        timer = setTimeout(() => {
            fn.apply(this, arguments)
        }, wait)
    }
}
```

## 简单的节流函数

```js
// 简单的节流函数

function throttle(fn, wait) {
    let prev = new Date();
    return function () {
        const args = arguments;
        const now = new Date();
        if (now - prev > wait) {
            fn.apply(this, args);
            prev = new Date();
        }
    }
}

// 通过第三个参数来切换模式

const throttle = function (fn, delay, isDebounce) {
    let timer
    let lastCall = 0
    return function (...args) {
        if (isDebounce) {
            if (timer) clearTimeout(timer)
            timer = setTimeout(() => {
                fn(...args)
            }, delay)
        } else {
            const now = new Date().getTime()
            if (now - lastCall < delay) return
            lastCall = now
            fn(...args)
        }
    }
}
```

## 解构常用方法合集

- 解构合并两个对象

```js
const obj1 = { a: 0 };
const obj2 = { b: 1 };

const obj = {...obj1, ...obj2};
// obj => { a: 0, b: 1 }
```

- 解构对象属性别名

```js
const obj = { a: 0, b: 1, c: 2 };
const { a, b: d, c: e } = obj;
// a d e => 0 1 2
```

- 解构对象属性默认值

当c不存在的时候默认赋值为3

```js
const obj = { a: 0, b: 1 };
const { a, b, c = 3 } = obj;

// a => 0
// b => 1
// c => 3
```

- 解构删除对象属性方法

```js
const obj = { a: 0, b: 1, c: 2 }; // 只想拿b和c
const { a, ...rest } = obj;

// rest => { b: 1, c: 2 }
```

- 解构数据单数据转对象

```js
let [a] = [{name:"swr",age:28}]

// a => {name:"swr",age:28}
```

- 解构赋值给已声明变量

```js
let name,age
// 需要用圆括号，包裹起来
({name,age} = {name:"swr",age:28})

// name => swr
// age => 28
```

## 函数自执行方法

```js
const Func = function() {}(); // 常用

(function() {})(); // 常用
(function() {}()); // 常用
[function() {}()];

+ function() {}();
- function() {}();
~ function() {}();
! function() {}();

new function() {};
new function() {}();
void function() {}();
typeof function() {}();
delete function() {}();

1, function() {}();
1 ^ function() {}();
1 > function() {}();
```

## Object.create的基本实现原理

```js
// 思路：将传入的对象作为原型
function create(obj) {
    function F() {}
    F.prototype = obj
    return new F()
}
```

## JavaScript对象深拷贝

拷贝内容不包含原型链

```js
function deepClone(obj) {
    let objStack = obj instanceof Array ? [] : {}
    for (let i in obj) {
        if (obj.hasOwnProperty(i)) {
            objStack[i] = typeof obj[i] === 'object' ? deepClone(obj[i]) : obj[i]
        }
    }
    return objStack;
}
```

拷贝内容包含原型链

是将原型链内容拷贝在对象上，使其优先被使用并未改变原型链上的内容。

```js
function deepClone(obj) {
    let objStack = obj instanceof Array ? [] : {}
    for (let i in obj) {
        objStack[i] = typeof obj[i] === 'object' ? deepClone(obj[i]) : obj[i]
    }
    return objStack;
}
```

## 使用filter和some快速筛选指定数据内容

```js
// 数据内容
var data = [
    {
        "nickname": "悦悦",
        "score": 6,
        "replay": "回复"
    },
    {
        "nickname": "悦悦",
        "score": 5,
        "replay": "未回复"
    },
    {
        "nickname": "悦悦",
        "score": 4,
        "replay": "未回复"
    }
];

// 筛选条件
var criteria = [
    {
        name: 'nickname',
        value: '悦悦'
    },
    {
        name: 'replay',
        value: '未回复'
    },
    {
        score: 'score',
        value: 4
    }
];

// 筛选方法
var results = data.filter(value => !criteria.some(val => val.value !== value[val.name]));

console.log(results);  // { "nickname": "悦悦","score": 4,"replay": "未回复"}
```

## 使用索引或者映射实现switch语句

```js
const cars = new Map()
  .set('usa', ['Ford', 'Dodge'])
  .set('france', ['Renault', 'Peugeot'])
  .set('italy', ['Fiat']);

const getCarsByState = (state) => {
  return cars.get(state) || [];
}

console.log(getCarsByState()); // 输出 []
console.log(getCarsByState('usa')); //输出 ['Ford', 'Dodge']
console.log(getCarsByState('italy')); // 输出 ['Fiat']
```

或者

```js
const carState = {
  usa: ['Ford', 'Dodge'],
  france: ['Renault', 'Peugeot'],
  italy: ['Fiat']
};

const getCarsByState = (state) => {
  return carState[state] || [];
}

console.log(getCarsByState()); // 输出 []
console.log(getCarsByState('usa')); // 输出 ['Ford', 'Dodge']
console.log(getCarsByState('france')); // 输出 ['Renault', 'Peugeot']
```

##  使用some匹配部分条件

```js
const cars = [
  { model: 'renault', year: 1956 },
  { model: 'peugeot', year: 1968 },
  { model: 'ford', year: 1977 }
];

const checkForAnyModel = (model) => {
  return cars.some(car => car.model === model);
}

console.log(checkForAnyModel('renault')); // 输出 true
```

## every或find实现匹配所有条件

```js
const cars = [
  { model: 'renault', year: 1956 },
  { model: 'peugeot', year: 1968 },
  { model: 'ford', year: 1977 }
];
```

every方式

```js
const checkEveryModel = (model) => {
  return cars.every(car => car.model === model);
}

console.log(checkEveryModel('renault')); // 输出 false
```

find方式

```js
const checkEveryModel = (model) => {
  return cars.find(car => car.model !== model) === undefined;
}

console.log(checkEveryModel('renault')); // 输出 false
```

两者的表现是一致的，因为两个函数都为数组中的每一个元素执行了回调，并且在找到一个 falsy 项时立即返回 false。

## includes实现多条件判断

```js
const checkCarModel = (model) => {
    const models = ['peugeot', 'renault'];

    if(models.includes(model)) {
    console.log('model valid');
    }
}

checkCarModel('renault'); // 输出 'model valid'
```

## instanceof实现原理

利用`Object.getPrototypeOf()`判断原型结构和Array.prototype原型对比判断是否相同。

```js
var instanceof = function (left, right) {
    let proto = Object.getPrototypeOf(left)
    while (true) {
        if (proto == null) return false
        if (proto === right.prototype) {
            return true
        }
        proto = Object.getPrototypeOf(proto)
    }
}
```

## JSON.stringify()替换输出内容

```js
const obj = { a: 1, b: 2, c: 3, d: { e: 4 } }; // `replacer` 使每个数字的值加 1。

JSON.stringify(obj, function replacer(key, value) {
    if (typeof value === 'number') {
        return value + 1;
    }
    return value;
});
```

输出：

```js
'{"a":2,"b":3,"c":4,"d":{"e":5}}'
```

## 最简单JS的去重方式 （重灾区）

es6的new Set()方式

```js
let array = [0, 3, 4, 5, 3, 4, 7, 8, 2, 2, 5, 4, 6, 7, 8, 0, 2, 0, 90];

[...new Set(array)]
```

es5的Array filter()

```js
[1, 3, 4, 5, 1, 2, 3, 3, 4, 8, 90, 3, 0, 5, 4, 0].filter(function (elem, index, Array) {
  return index === Array.indexOf(elem);
})
```

## 求最大值/最小值

```
let arr = [1, 2, 3, 4, 5]

console.log(arr.reduce((prev, cur) => Math.max(prev, cur))); // 5
console.log(arr.reduce((prev, cur) => Math.min(prev, cur))); // 1
```

## 高阶函数实现缓存(备忘模式)

比如有个函数：

```js
var add = function(a) {
    return a + 1;
}
```

每次运行add(1)的时候都会输出2，但是输入1每次还是会计算一下1+1，如果是开销很大的操作的话就比较消耗性能了，这里其实可以对这个计算进行一次缓存。
所以这里可以利用高阶函数的思想来实现一个简单的缓存，我可以在函数内部用一个对象存储输入的参数，如果下次再输入相同的参数，那就比较一下对象的属性，把值从这个对象里面取出来。

```js
const memorize = function(fn) {
  const cache = {}
  return function(...args) {
    const _args = JSON.stringify(args)
    return cache[_args] || (cache[_args] = fn.apply(fn, args))
  }
}
const add = function(a) {
  return a + 1
}
const adder = memorize(add)
adder(1)    // 2    cache: { '[1]': 2 }
adder(1)    // 2    cache: { '[1]': 2 }
adder(2)    // 3    cache: { '[1]': 2, '[2]': 3 }
```

用JSON.stringify把传给 adder 函数的参数变成了字符串，并且把它当做 cache 的 key，将 add 函数运行的结果当做 value 传到了 cache 里面，这样 memorize 的匿名函数运行的时候会返回`cache[_args]`，如果`cache[_args]`不存在的话就返回`fn.apply(fn,args)`，把`fn.apply(fn, arguments)`赋值给`cache[_args]`并返回。
注意：cache不可以是Map，因为Map的键是使用===比较的，`[1]！==[1]`，因此即使传入相同的对象或者数组，那么还是被存为不同的键。

```js
const memorize = function(fn) {        //  X 错误示范
  const cache = new Map()
  return function(...args) {
    return cache.get(args) || cache.set(args, fn.apply(fn, args)).get(args)
  }
}
const add = function(a) {
  return a + 1
}
const adder = memorize(add)
adder(1)    // 2    cache: { [ 1 ] => 2 }
adder(1)    // 2    cache: { [ 1 ] => 2, [ 1 ] => 2 }
adder(2)    // 3    cache: { [ 1 ] => 2, [ 1 ] => 2, [ 2 ] => 3 }
```

## 优雅的向下取整

向下取整有很多种方式，做常用的，是调用Math的方法，如下图的例子

```js
let num = 1.23
let num1 = Math.floor(num);
console.log(num1); //1
```

但是下面有一种更加优雅的方式

```js
let num = 1.23
let num1 = num | 0;
console.log(num1)  // 1
```

这种方式更加简洁，这种方式的原理是来源于js的位运算，这边的 | 不是逻辑或，是按或运算

注意点：

Math.floor(NaN)返回的是NaN，但是或零返回的是0；
Math.floor(Infinity)返回的是Infinity，但是或零返回的是0；
补充:评论中补充了一个～～也可以向下取整，确实更加优雅，推荐，关于这个原理有兴趣的朋友可以自己去看一下，～是取反操作符，我试了一下1.234取反是-2，在取反就是1，不过以上注意点变了

~~NaN等于0，这个原理就是js会先调用Number，把NaN转化成false，false取反就是-1，在取反就是0。


## JS 对象转 url 查询字符串

```js
const objectToQueryString = (obj) => Object.keys(obj).map((key) => `${encodeURIComponent(key)}=${encodeURIComponent(obj[key])}`).join('&'); objectToQueryString({name: 'Jhon', age: 18, address: 'beijing'}) // name=Jhon&age=18&address=beijing
```

## 随机生成六位数字验证码

```js
const code = Math.floor(Math.random() * 1000000).toString().padStart(6, "0") // 942377
```

## 手动实现一个new方法

**new步骤**

模拟new操作前，要先知道new操作是发生了什么，就拿new Object()举例:

**创建一个新对象**

- 把新对象的原型指向构造函数的prototype
- 把构造函数里的this指向新对象
- 返回这个新对象

构造函数：

先准备一个构造函数来new使用。

```js
function constructorFunction(name, age){
  this.name = name;
  this.age = age;
}
constructorFunction.prototype.say = function(){
  return 'Hello '+ this.name
}
```

原生new：

```js
var obj = new constructorFunction('willian', 18)

console.log(obj.name, obj.age);//'willian', 18
console.log(obj.say())//Hello willian
```

模拟new

使用：`newNew(constructor, arg1, arg2, ..)` 第0个参数传入构造函数，1~n个参数是构造函数的形参。
使用上面的构造函数试一下：

```js
function newNew(){
    var newObj = {}
    // 1. 创建一个新对象
    var Con = [].shift.call(arguments)
    // 得到构造函数
    newObj.__proto__ = Con.prototype;
    // 2. 把新对象的原型指向构造函数的prototype
    var res = Con.apply(newObj, arguments)
    // 3. 把构造函数里的this指向新对象
    return typeof res === 'object' ? res : newObj;
    // 4. 返回新对象
}

var obj = newNew(constructorFunction, 'willian', 18)
console.log(obj.name, obj.age);//'willian', 18
console.log(obj.say())//Hello willian
```

## 生成随机ID

在原型设计时经常使用的创建ID功能。但是我在实际项目中看到有人使用它。其实这并不安全

```js
// 生成长度为11的随机字母数字字符串
Math.random().toString(36).substring(2);
// hg7znok52x
```

## 生成随机十六进制代码（生成随机颜色）

使用JavaScript简洁代码生成随机十六进制代码

```js
// 生成随机十六进制代码 如：'#c618b2'
'#' + Math.floor(Math.random() * 0xffffff).toString(16).padEnd(6, '0');
```

## ES7数组快速去重

```
[...new Set(arr)]
```

## 创建过去七天的数组

使用ES7快速创建过去七天的数组

```js
[...Array(7).keys()].map(days => new Date(Date.now() - 86400000 * days));
```

## ES6快速处理URL地址参数

```js
var urlParams = new URLSearchParams(window.location.search);

console.log(urlParams.has('post')); // true
console.log(urlParams.get('action')); // "edit"
console.log(urlParams.getAll('action')); // ["edit"]
console.log(urlParams.toString()); // "?post=1234&action=edit"
console.log(urlParams.append('active', '1')); // "?post=1234&action=edit&active=1"
```

## ES6快速合并对象内容并能相互替换

```js
const person = { name: 'David Walsh', gender: 'Male' };
const tools = { computer: 'Mac', editor: 'Atom' };
const attributes = { handsomeness: 'Extreme', hair: 'Brown', eyes: 'Blue' };

const summary = {...person, ...tools, ...attributes};
```

注：如果对象键值一致会以后先后顺序进行覆盖合并

## ES6数组快速去重

```js
var j = [...new Set([1, 2, 3, 3])]

// >> [1, 2, 3]
```

## ES6函数参数设置默认空值返回错误

```js
const isRequired = () => { throw new Error('param is required'); };

const hello = (name = isRequired()) => { console.log(`hello ${name}`) };

// This will throw an error because no name is provided
hello();

// This will also throw an error
hello(undefined);

// These are good!
hello(null);
hello('David');
```

## 实现两个字符串进行加法计算

```js
function sumStrings(a,b) {
    var res = '', temp = 0;
    a = a.split('');
    b = b.split('');
    while (a.length || b.length || temp) {
        temp += ~~a.pop() + ~~b.pop();
        res = (temp % 10) + res;
        temp = temp > 9;
        // 判断 temp 是否大于 10，若是则将 temp 赋值为 true，等等，为什么要赋值成布尔值，不要着急，魔法即将发生。
        // 在两个大数中的一个还有数字没有参与运算，或者前一次运算发生进位后，进行下一次循环。
        // 接着除了对新的两个数字相加还要加上 temp，若上次发生了进位，则此时 temp 为 true，
        // Js因为存在隐式转换，所以 true 转换为 1，我们借用 Js 的类型转换，完成了逻辑上的逢10进1操作。
    }
    return res.replace(/^0+/, '');
}

// Input
sumStrings('130', '50'))
```

## 实现两个字符串进行乘法计算

```js
function multiply(a, b) {
    return a.split('').reduceRight((p, a, i) =>
        b.split('').reduceRight((p, b, j) => {
            const mul = (a - '0') * (b - '0');
            const p1 = i + j;
            const p2 = p1 + 1;
            const sum = mul + (p[p2] || 0);

            p[p1] = (p[p1] || 0) + Math.floor(sum / 10);
            p[p2] = sum % 10;

            return p;
        }, p), []).join('').replace(/^0+(?=\d)/, '');
}

// Input
multiply('30', '20')
```

## 两种简单的数组去重方案

- filter去除数组方法

```js
function removeDuplicates(arr) {
  return arr.filter((item, pos) => arr.indexOf(item) === pos)
}
```

- Set去除数组方法

```js
function removeDuplicates(arr) {
   return [...new Set(arr)];
}
```

## 获取选中内容并包裹标签更换内容

```js
document.getElementById('execute').addEventListener('click', function() {
    var range = window.getSelection().getRangeAt(0);
    var span = document.createElement('span');

    span.className = 'highlight';
    span.appendChild(range.extractContents());
    range.insertNode(span);
});
```

```css
.highlight { background-color: yellow; }
```

```html
<div id="test">
    Select any part of <b>this text and</b> then click 'Run'.
</div>

<button id="execute">Run</button>
```

## 深究setTime循环出现的问题

- 普通写法

```js
for (var i = 0; i < 5; i++) {
    (function(j) {
        setTimeout(function() {
            console.log(new Date, j);
        }, 1000 * j));  // 这里修改 0~4 的定时器时间
    })(i);
}
```

- Promise写法

```js
const tasks = []; // 这里存放异步操作的 Promise
const output = (i) => new Promise((resolve) => {
    setTimeout(() => {
        console.log(new Date, i);
        resolve();
    }, 1000 * i);
});

// 生成全部的异步操作
for (var i = 0; i < 5; i++) {
    tasks.push(output(i));
}
```

- async await写法

```js
const sleep = (timeountMS) => new Promise((resolve) => {
    setTimeout(resolve, timeountMS);
});

(async () => {  // 声明即执行的 async 函数表达式
    for (var i = 0; i < 5; i++) {
        await sleep(1000);
        console.log(new Date, i);
    }
})();
```

## 判断指定内容是否存在

```js
const fruits = [
    {
        name: 'apple',
        color: 'red'
    },
    {
        name: 'banana',
        color: 'yellow'
    },
    {
        name: 'grape',
        color: 'purple'
    }
];

function test() {
    let isAllRed = true;

    // 条件：所有水果都是红色
    for (let f of fruits) {
        if (!isAllRed) break;
        isAllRed = (f.color == 'red');
    }

    console.log(isAllRed); // false
}
```

简单的写法

```js
var fruits = [
    { name: 'apple', color: 'red' },
    { name: 'banana', color: 'yellow' },
    { name: 'grape', color: 'purple' }
];

function test() {
  var isAllRed = fruits.every(function(f){
      return f.color == 'red'
  });

  console.log(isAllRed); // false
}
```

或

```js
var fruits = [
    { name: 'apple', color: 'red' },
    { name: 'banana', color: 'yellow' },
    { name: 'grape', color: 'purple' }
];

function test() {
  // 条件：任何一个水果是红色
  var isAnyRed = fruits.some(f => f.color == 'red');

  console.log(isAnyRed); // true
}
```

## 通过数组进行多条件并存判断

```js
// condition
function test(fruit) {
  if (fruit == 'apple' || fruit == 'strawberry') {
    console.log('red');
  }
}
```

```js
function test(fruit) {
  const redFruits = ['apple', 'strawberry', 'cherry', 'cranberries'];

  if (redFruits.includes(fruit)) {
    console.log('red');
  }
}
```

## 创建文本DOM方法

```
document.createTextNode('Hello');
```

## 字符串转数字快捷方法

```js
var str = '999';
var num = str * 1; //999

var str = '999';
var num = str - 0; //999
```

## 向下取整快捷方法

```js
var num = ~~1.23232656; //  1

var num = 563.933333 >> 0; //  563
```

## 柯里化正则验证写法

```js
// 简单实现，参数只能从右到左传递
function createCurry(func, args) {

    var arity = func.length;
    var args = args || [];

    return function() {
        var _args = [].slice.call(arguments);
        [].push.apply(_args, args);

        // 如果参数个数小于最初的func.length，则递归调用，继续收集参数
        if (_args.length < arity) {
            return createCurry.call(this, func, _args);
        }

        // 参数收集完毕，则执行func
        return func.apply(this, _args);
    }
}

function check(targetString, reg) {
    return reg.test(targetString);
}

var _check = createCurry(check);

var checkPhone = _check(/^1[34578]\d{9}$/);
var checkEmail = _check(/^(\w)+(\.\w+)*@(\w)+((\.\w+)+)$/);

checkPhone('183888888');
checkEmail('xxxxx@test.com');
```

## 函数传参转柯里化函数传参

普通的函数传参方式

```js
function add(a, b, c) {
    return a + b + c;
}

add(1, 2, 3);
```

柯里化函数传参方式

```js
function add(a) {
    return function(b) {
        return function(c) {
            return a + b + c;
        }
    }
}

add(1)(2)(3);
```

## ES6类的静态成员

```js
class Person {
    constructor(name) {
        this.name = name;
    }
    static create(name) {
        return new Person(name);
    }
}

let beauty = Person.create("Jenny");
beauty.create('lee') // TypeError
```

## ES6类的继承

回顾 ES6 之前如何实现继承？常用方式是通过原型链、构造函数以及组合继承等方式。

ES6 的类使用熟悉的extends关键字指定类继承的函数，并且可以通过surpe()方法访问父类的构造函数。

例如继承一个 Person 的类：

```js
class Friend extends Person {
    constructor(name, phone){
        super(name)
        this.phone = phone
    }
}

let myfriend = new Friend('lee',2233)
console.log(myfriend) // Friend { name: 'lee', phone: 2233 }
```

Friend 继承了 Person，术语上称 Person 为基类，Friend 为派生类。

需要注意的是，surpe()只能在派生类中使用，它负责初始化 this，所以派生类使用 this 之前一定要用surpe()。

## 继承内建对象

ES6 的类继承可以继承内建对象（Array、Set、Map 等），继承后可以拥有基类的所有内建功能。例如：


```js
class MyArray extends Array {
}

let arr = new MyArray(1, 2, 3, 4);
let subarr = arr.slice(1, 3);

console.log(arr.length) // 4
console.log(arr instanceof MyArray) // true
console.log(arr instanceof Array) // true
console.log(subarr instanceof MyArray) // true
```
注意到上例中，不仅 arr 是派生类 MyArray 的实例，subarr 也是派生类 MyArray 的实例，内建对象继承的实用之处是改变返回对象的类型。

浏览器引擎背后是通过`[Symbol.species]`属性实现这一行为，它被用于返回函数的静态访问器属性，内建对象定义了`[Symbol.species]`属性的有 Array、ArrayBuffer、Set、Map、Promise、RegExp、Typed arrays。

## 继承表达式的类

目前extends可以继承类和内建对象，但更强大的功能从表达式导出类！

这个表达式要求可以被解析为函数并具有`[[Construct]]`属性和原型，示例如下：

```js
function Sup(val) {
    this.value = val
}

Sup.prototype.getVal = function () {
    return 'hello' + this.value
}

class Derived extends Sup {
    constructor(val) {
        super(val)
    }
}

let der = new Derived('world')
console.log(der) // Derived { value: 'world' }
console.log(der.getVal()) // helloworld
```

## 只能继承的抽象类

ES6 引入new.target元属性判断函数是否通过new关键字调用。类的构造函数也可以通过new.target确定类是如何被调用的。

可以通过new.target创建抽象类（不能实例化的类），例如：

```js
class Abstract  {
    constructor(){
        if(new.target === Abstract) {
            throw new Error('抽象类（不能直接实例化）')
        }
    }
}

class Instantiable extends Abstract {
    constructor() {
        super()
    }
}

// let abs = new Abstract() // Error: 抽象类（不能直接实例化）
let abs = new Instantiable()
console.log(abs instanceof Abstract) // true
```

虽然不能直接使用 Abstract 抽象类创建实例，但是可以作为基类派生其它类。

## ES6可计算的成员名称

```js
let methodName = 'sayName'

class Person {
    constructor(name) {
        this.name = name;
    }

    [methodName + 'Default']() {
        console.log(this.name);
    }

    get [methodName]() {
        return this.name
    }

    set [methodName](str) {
        this.name = str
    }
}

let friend = new Person("Jenny");

// 方法
friend.sayNameDefault(); // Jenny
// 访问器属性
friend.sayName = 'lee'
console.log(friend.sayName) // lee
```

## ES6访问器属性

```javascript
class Person {
    constructor(name) {
        this.name = name;
    }
    get value () {
        return this.name + this.age
    }
    set value (num) {
        this.age = num
    }
}

let friend = new Person("Jenny");
// 调用的是 setter
friend.value = 18
// 调用的是 getter
console.log(friend.value) // Jenny18
```

## 原生js惯性滚动与回弹效果

```html
<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8"/>
    <meta name="Keywords" content=""/>
    <meta name="Description" content=""/>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/>
    <meta name="viewport" content="width=device-width,initial-scale=1,user-scalable=no"/>
    <meta name="apple-mobile-web-app-capable" content="yes"/>
    <meta content="telephone=no" name="format-detection"/>
    <meta content="email=no" name="format-detection"/>
    <title>Document</title>
    <style>
        body {
            margin: 0;
            padding: 0;
        }

        div {
            position: relative;
            width: 200px;
            height: 300px;
            margin: 3em auto;
            border: 1px solid #CCC;
            overflow: hidden;
            -webkit-user-select: none;
            user-select: none;
        }

        ol {
            width: 100%;
        }

        ol > li {
            height: 30px;
        }
    </style>
</head>

<body>
<div>
    <ol>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
    </ol>
</div>
<script>
    function myScroll(ctx) {
        var ol = ctx.firstElementChild || ctx.firstChild,
                offset = 50,//最大溢出值
                cur = 0,//列表滑动位置
                isDown = false,
                vy = 0,//滑动的力度
                fl = 150,//弹力,值越大,到度或到顶后,可以继续拉的越远
                isInTransition = false;//是否在滚动中

        ctx.addEventListener("mousedown", function (e) {
            if (isInTransition)return;//如果在滚动中，则中止执行
            clearTimeout(this._timer);//清除定时器
            vy = 0;
            this._oy = e.clientY - cur;//计算鼠标按下位置与列表当前位置的差值,列表位置初始值为0
            this._cy = e.clientY;//鼠标按下的位置
            this._oh = this.scrollHeight;//列表的高度
            this._ch = this.clientHeight;//容器的高度
            this._startTime = e.timeStamp;//鼠标按下时的时间戳
            isDown = true;//鼠标是否有按下，主要防止用户是从容器外开始滑动的

        });

        ctx.addEventListener("mousemove", function (e) {
            if (isDown) {//如果鼠标是从容器里开始滑动的
                if (e.timeStamp - this._startTime > 40) {//如果是慢速滑动，就不会产生力度，列表是跟着鼠标移动的
                    this._startTime = e.timeStamp;//慢速滑动不产生力度，所以需要实时更新时间戳
                    cur = e.clientY - this._oy;//列表位置应为 鼠标当前位置减去鼠标按下时与列表位置的差值,如:列表初始位置为0,鼠标在 5的位置按,那么差值为 5,此处假如鼠标从5滑动到了4,向上滑,cur = 4-5 =-1  ,假如鼠标从5滑动到了6,向下滑,cur= 6 - 5 = 1


                    if (cur > 0) {//如果列表位置大于0,既鼠标向下滑动并到顶时
                        cur *= fl / (fl + cur);//列表位置带入弹力模拟,公式只能死记硬背了,公式为:位置 *=弹力/(弹力+位置)
                    }else if (cur < this._ch - this._oh) {//如果列表位置小于 容器高度减列表高度(因为需要负数,所以反过来减),既向上滑动到最底部时。
                        //当列表滑动到最底部时,cur的值其实是等于 容器高度减列表高度的,假设窗口高度为10,列表为30,那此时cur为 10 - 30 = -20,但这里的判断是小于,所以当cur<-20时才会触发,如 -21;
                        cur += this._oh - this._ch;//列表位置加等于 列表高度减容器高度(这是与上面不同,这里是正减,得到了一个正数) ,这里 cur 为负数,加上一个正数,延用上面的假设,此时 cur = -21 + (30-10=20) = -1 ,所以这里算的是溢出数

//                        console.log(cur);
                        cur = cur * fl / (fl - cur) - this._oh + this._ch;//然后给溢出数带入弹力,延用上面的假设,这里为   cur = -1 * 150 /(150 - -1 = 151)~= -0.99 再减去 30  等于 -30.99  再加上容器高度 -30.99+10=-20.99  ,这也是公式,要死记。。
                    }
                    setPos(cur);//移动列表
                }
                vy = e.clientY - this._cy;//记录本次移动后,与前一次鼠标位置的滑动的距离,快速滑动时才有效,慢速滑动时差值为 1 或 0,vy可以理解为滑动的力度

//                console.log(vy);
                this._cy = e.clientY;//更新前一次位置为现在的位置,以备下一次比较
            }

        }, false);

        ctx.addEventListener("mouseleave", mleave, false);

        ctx.addEventListener("mouseup", mleave, false);

        function setPos(y) {//传们列表y轴位置,移动列表
            ol.style.transform = "translateY(" + y + "px) translateZ(0)";
        }

        function ease(target) {
            isInTransition = true;
            ctx._timer = setInterval(function () {//回弹算法为  当前位置 减 目标位置 取2个百分点 递减
                cur -= (cur - target) * 0.2;
                if (Math.abs(cur - target) < 1) {//减到 当前位置 与 目标位置相差小于1 之后直接归位
                    cur = target;
                    clearInterval(ctx._timer);
                    isInTransition = false;
                }
                setPos(cur);
            }, 20);
        }

        function mleave(e) {
            if (isDown) {
                isDown = false;
                console.log(vy);
                var t = this,
                        friction = ((vy >> 31) * 2 + 1) * 0.5,//根据力度套用公式计算出惯性大小,公式要记住
                        oh = this.scrollHeight - this.clientHeight;
                this._timer = setInterval(function () {//
                    vy -= friction;//力度按 惯性的大小递减
                    cur += vy;//转换为额外的滑动距离
                    setPos(cur);//滑动列表

                    if (-cur - oh > offset) {//如果列表底部超出了
                        clearTimeout(t._timer);
                        ease(-oh);//回弹
                        return;
                    }
                    if (cur > offset) {//如果列表顶部超出了
                        clearTimeout(t._timer);
                        ease(0);//回弹
                        return;
                    }
                    if (Math.abs(vy) < 1) {//如果力度减小到小于1了,再做超出回弹
                        clearTimeout(t._timer);
                        if (cur > 0) {
                            ease(0);
                            return;
                        }
                        if (-cur > oh) {
                            ease(-oh);
                            return;
                        }
                    }
                }, 20);
            }
        }
    }

    myScroll(document.querySelector("div"));
</script>
</body>

</html>
```


## 中文和字母排序方法

使用localeCompare进行中文排序

- 定义：用本地特定的顺序来比较两个字符串。
- 语法：stringObject.localeCompare(target)
- 参数：target——要以本地特定的顺序与 stringObject 进行比较的字符串。
- 返回值：说明比较结果的数字。
    - （1）如果 stringObject 小于 target，则 localeCompare() 返回小于 0 的数。
    - （2）如果 stringObject 大于 target，则该方法返回大于 0 的数。
    - （3）如果两个字符串相等，或根据本地排序规则没有区别，该方法返回 0。

　　说明：把 `<` 和 `>` 运算符应用到字符串时，它们只用字符的 Unicode 编码比较字符串，而不考虑当地的排序规则。以这种方法生成的顺序不一定是正确的。localeCompare() 方法提供的比较字符串的方法，考虑了默认的本地排序规则。ECMAscript 标准并没有规定如何进行本地特定的比较操作，它只规定该函数采用底层操作系统提供的排序规则。

实例：

1、可以使用localeCompare() 方法来实现中文按照拼音排序，方法相当简单

```javascript
var array = ['白鸽', '麻雀', '大象', '狗', '猫', "鸡"];
array = array.sort(function compareFunction(item1, item2) {
    return item1.localeCompare(item2);
});
//["白鸽", "大象", "狗", "鸡", "麻雀", "猫"]
```

而且可以通过如下代码实现中文按照拼音排序，并且可以将中文按照a,b,c,d……进行区分。代码如下：

```javascript
function pySegSort(arr,empty) {
    if(!String.prototype.localeCompare)
        return null;

    var letters = "*abcdefghjklmnopqrstwxyz".split('');
    var zh = "阿八嚓哒妸发旮哈讥咔垃痳拏噢妑七呥扨它穵夕丫帀".split('');

    var segs = [];
    var curr;
    $.each(letters, function(i){
        curr = {letter: this, data:[]};
        $.each(arr, function() {
            if((!zh[i-1] || zh[i-1].localeCompare(this) <= 0) && this.localeCompare(zh[i]) == -1) {
                curr.data.push(this);
            }
        });
        if(empty || curr.data.length) {
            segs.push(curr);
            curr.data.sort(function(a,b){
                return a.localeCompare(b);
            });
        }
    });
    return segs;
}
console.log(JSON.stringify(pySegSort(['白鸽', '麻雀','黑','大象', '狗', '猫','妈妈','马', "鸡",'瘦','胖'])));
```

结果显示为：`[{"letter":"b","data":["白鸽"]},{"letter":"d","data":["大象"]},{"letter":"g","data":["狗"]},{"letter":"h","data":["黑"]},{"letter":"j","data":["鸡"]},{"letter":"m","data":["妈妈","麻雀","马","猫"]},{"letter":"p","data":["胖"]},{"letter":"s","data":["瘦"]}]；`通过这个就可以写一个电话薄，像现在手机上面的，通过人名来进行分组、排序，之后再通过循环和布局就可以实现电话薄的功能。

2、实现字母、数字的混合排序：

```javascript
var d = [1,2,3,'a','k','b','d',10,20,'c']
d.sort(function(a,b){
    var c = isFinite(a), // 如果 number 是有限数字（或可转换为有限数字），那么返回 true。否则，如果 number 是 NaN（非数字），或者是正、负无穷大的数，则返回 false。
        d = isFinite(b);
    return (c != d && d - c) || a > b;
})
console.log(d);
//[1, 2, 3, 10, 20, "a", "b", "c", "d", "k"]
```


isFinite() 判断a、b是否是数字。

return 后面的语句：

`c != d && c - d`  如果c和d不相等 ，也就是说比较的值不是同一类型。那就比较 c-d的值是1还是-1（中间进行了隐式类型转换）

如果c == d 也就是说c、d是同一类型的值，c、d可能都是字母，也可能都是数字。这里就可以直接比较大小了（都是字母的话不能直接做减法）。

isFinite() 函数用于检查其参数是否是无穷大。如果 number 是有限数字（或可转换为有限数字），那么返回 true。否则，如果 number 是 NaN（非数字），或者是正、负无穷大的数，则返回 false。

## DOM事件绑定方法

```javascript
function DOMExtend(name, fn) {
    if (typeof (HTMLElement) != "undefined") {
        HTMLElement.prototype[name] = fn;
    } else {
        var _getElementById = document.getElementById;
        document.getElementById = function (id) {
            var _elem = _getElementById(id);
            eval("_elem." + name + "=" + fn);
            return _elem;
        };
        var _getElementByTagName = document.getElementsByTagName;
        document.getElementsByTagName = function (tag) {
            var _elem = _getElementByTagName(tag);
            var len = _elem.length;
            for (var i = 0; i < len; i++) {
                eval("_elem[" + i + "]." + name + "=" + fn);
            }
            return _elem;
        };
        var _createElement = document.createElement;
        document.createElement = function (tag) {
            var _elem = _createElement(tag);
            eval("_elem." + name + "=" + fn);
            return _elem;
        };

        var _documentElement = document.documentElement;
        eval("_documentElement." + name + "=" + fn);

        var _documentBody = document.body;
        eval("_documentBody." + name + "=" + fn);
    }
}
DOMExtend('add', function () {
    console.log(this, 123);
});
```

## JS原生手写on和off绑定解绑方法

```javascript
(function(){
    function addEvent(){
        if(!(this instanceof addEvent)){
            return new addEvent();
        }
    }
    addEvent.prototype = {
        eventList: [],
        store: [],
        trigger: function(e){
            for(var item in this.store){
                if (this.store.hasOwnProperty(item)) {
                    var type = this.store[item].name.substr(0,1);
                    var name = /\#|\./.test(this.store[item].name) ? this.store[item].name.substr(1) : this.store[item].name;
                    if(type == '#'){
                        if(e.target.id == name && e.type == this.store[item].type){
                            this.store[item].fn();
                        }
                    }else if(type == '.'){
                        if(e.target.className == name && e.type == this.store[item].type){
                            this.store[item].fn();
                        }
                    }else{
                        if(e.target.localName == name && e.type == this.store[item].type){
                            this.store[item].fn();
                        }
                    }
                }
            }
        },
        on: function(event,ele,fn){
            this.store.push({
                name: ele,
                type: event,
                fn: fn
            })
            var existStatus = false;
            for(var item in this.eventList){
                if(this.eventList[item] == event){
                    existStatus = true;
                }
            }
            if(!existStatus){
                this.eventList.push(event);
                if (document.addEventListener) {
                    document.addEventListener(event, this.trigger.bind(this));
                } else if (document.attachEvent) {
                    document.attachEvent('on' + event , this.trigger.bind(this));
                } else {
                    return false;
                }
            }
        },
        off: function(event,ele){
            for(var item in this.store){
                if (this.store.hasOwnProperty(item)) {
                    if(this.store[item].name == ele && this.store[item].type == event){
                        this.store.splice(item,1);
                    }
                }
            }
        }
    }

    window.addEvent = addEvent();
})()
```


## 阻止微信上拉底部回弹效果

```javascript
document.body.addEventListener('touchmove', function (e) {
    e.preventDefault();
}, {passive: false});
```
如果不加passive:false,在 ios 上是不能起作用的。


## 监听页面属性或者结构发生变化触发

```html
<div id="a"></div>
<button id="b">改变</button>
```

```javascript
var MutationObserver = window.MutationObserver || window.WebKitMutationObserver || window.MozMutationObserver; //浏览器兼容
var config = {
    attributes: true,
    childList: true
}
var $a = document.querySelector('#a');
var $b = document.querySelector('#b');

var observer = new MutationObserver(function (mutations) { //构造函数回调
    mutations.forEach(function (record) {
        if (record.type == "attributes") { //监听属性
            //do any code
            console.log('属性发生改变')
        }
        if (record.type == 'childList') { //监听结构发生变化
            //do any code
            console.log('结构发生改变')
        }
    });
});

observer.observe($a, config);

$b.onclick = function () {
    $a.className = 'game';
    $a.innerHTML = '<div></div>';
}
```

MutationObserver所观察的DOM变动（即上面代码的option对象），包含以下类型：

- childList：子元素的变动
- attributes：属性的变动
- characterData：节点内容或节点文本的变动
- subtree：所有下属节点（包括子节点和子节点的子节点）的变动

想要观察哪一种变动类型，就在option对象中指定它的值为true。需要注意的是，不能单独观察subtree变动，必须同时指定childList、attributes和characterData中的一种或多种。

除了变动类型，option对象还可以设定以下属性：

- attributeOldValue：值为true或者为false。如果为true，则表示需要记录变动前的属性值。
- characterDataOldValue：值为true或者为false。如果为true，则表示需要记录变动前的数据值。
- attributesFilter：值为一个数组，表示需要观察的特定属性（比如['class', 'str']）。

**disconnect方法和takeRecord方法**

disconnect方法用来停止观察。发生相应变动时，不再调用回调函数。

```javascript
observer.disconnect();
```

takeRecord方法用来清除变动记录，即不再处理未处理的变动。

```javascript
observer.takeRecord
```

**MutationRecord对象**

DOM对象每次发生变化，就会生成一条变动记录。这个变动记录对应一个MutationRecord对象，该对象包含了与变动相关的所有信息。Mutation Observer进行处理的一个个变动对象所组成的数组。

MutationRecord对象包含了DOM的相关信息，有如下属性：

- type:观察的变动类型（attribute、characterData或者childList）。
- target:发生变动的DOM对象。
- addedNodes:新增的DOM对象。
- removeNodes:删除的DOM对象。
- previousSibling:前一个同级的DOM对象，如果没有则返回null。
- nextSibling:下一个同级的DOM对象，如果没有就返回null。
- attributeName:发生变动的属性。如果设置了attributeFilter，则只返回预先指定的属性。
- oldValue:变动前的值。这个属性只对attribute和characterData变动有效，如果发生childList变动，则返回null。


## &&在JS中的另类用途

`&&`可用用来做代码增强避免出现某些变量不存在导致的报错

实例：

```javascript
function test(callback){
    callback && callback();
};

test();
test(function(){
    console.log('test');
});
```

当传参缺少函数的时候使用&&调用去判断可以避免出现报错，&&的前面如果不存在则不会往后走。

## ECMA-262规范定义的七种错误类型

- 第一种：Error

所有错误的基本类型，实际上不会被抛出。

- 第二种：EvalError

```js
throw new EvalError("That doesn’t evaluate.");
```

执行eval错误时抛出。

- 第三种：ReferenceError

```js
throw new ReferenceError("You didn’t cite your references properly.");
```

对象不存在是抛出。

- 第四种：RangeError

```js
throw new RangeError("Sorry, you just don’t have the range.");
```

数字超出边界时抛出。

- 第五种：SyntaxError

```js
throw new SyntaxError("I don’t like your syntax.");
```

出现语法错误时抛出。

- 第六种：TypeError

```js
throw new TypeError("What type of variable do you take me for?");
```

变量不是期望的类型时抛出。

- 第七种：URIError

```js
throw new URIError("Uri, is that you?");
```

给encodeURI（）等函数传递非法字符串时抛出。

## 强制触发JS错误提示并终止进程

```
throw new TypeError('First argument must be a String, HTMLElement, HTMLCollection, or NodeList');
```

## 可编辑DIV的DIV标签改为P标签

```javascript
document.execCommand("defaultParagraphSeparator", false, "p");
```

## 返回事件监听方法

```javascript
window.addEventListener("popstate", function(e) {
    ...
}, false);
```

禁止后退返回上一页实例:

```javascript
window.addEventListener("popstate", function(e) {
    window.history.forward();
}, false);
```

## Range操作详解

```javascript
var selection, range;
if (window.getSelection) {
    //现代浏览器
    selection = window.getSelection();
} else if (document.selection) {
    //IE
    selection = document.selection.createRange();
}

//Range对象
range = selection.getRangeAt(0);
```

range属性:

- collapsed => 如果范围的开始点和结束点在文档的同一位置，则为 true，即范围是空的，或折叠的。
- commonAncestorContainer => 范围的开始点和结束点的（即它们的祖先节点）、嵌套最深的 Document 节点。
- endContainer => 包含范围的结束点的 Document 节点。
- endOffset => endContainer 中的结束点位置。
- startContainer => 包含范围的开始点的 Document 节点。
- startOffset => startContainer中的开始点位置。

range操作:

```javascript
//选中区域的文字
var text = range.toString();

//选中区域的Element元素
var elem = range.commonAncestorContainer;
if(elem.nodeType != 1){
     elem = elem.parentNode;
}

//选中区域的html
var span = document.createElement('SPAN');
span.appendChild(range.cloneContents());

//选区是否为空
var isSelectionEmpty = false;
if (range.startContainer === range.endContainer) {
   if (range.startOffset === range.endOffset) {
       isSelectionEmpty = true;
   }
}
```

## 过滤粘贴特殊标签

```javascript
var nowContentText = text.replace(/<meta.+?>/, "");
nowContentText = nowContentText.replace(/<(div|p|a|i|span|em|h3)[^>]*>/gi,"<$1>");
nowContentText = nowContentText.replace(/<a>(.*?)<\/a>/gi, "$1");
nowContentText = nowContentText.replace(/<i>(.*?)<\/i>/gi, "$1");
nowContentText = nowContentText.replace(/<span>(.*?)<\/span>/gi,"$1");
nowContentText = nowContentText.replace(/<em>(.*?)<\/em>/gi, "$1");
nowContentText = nowContentText.replace(/<p>(.*?)<\/p>/gi, "$1");
nowContentText = nowContentText.replace(/<h1>(.*?)<\/h1>/gi, "$1");
nowContentText = nowContentText.replace(/<h2>(.*?)<\/h2>/gi, "$1");
nowContentText = nowContentText.replace(/<h3>(.*?)<\/h3>/gi, "$1");
nowContentText = nowContentText.replace(/<h4>(.*?)<\/h4>/gi, "$1");
nowContentText = nowContentText.replace(/<h5>(.*?)<\/h5>/gi, "$1");
var textData = nowContentText.split("</div>");
var nowTextData = [];
textData.forEach(function (data, index) {
    if (data !== "") {
        nowTextData.push(
            "<p>" +
            data.replace(
                /<div>|<\/div>|<br.*?>|<br.*?\/>|<span>|<\/span>/gi,
                ""
            ) +
            "</p>"
        );
    }
});
```

## 光标处插入内容

```javascript
function insertToRange(html){
    var sel,textRange;
    if (document.body.createTextRange) {
        if (document.selection) {
            textRange = document.selection.createRange()
        } else if (window.getSelection) {
            sel = window.getSelection()
            var range = sel.getRangeAt(0)

            // 创建临时元素，使得TextRange可以移动到正确的位置
            var tempEl = document.createElement("span")
            tempEl.innerHTML = "&#FEFF;"
            range.deleteContents()
            range.insertNode(tempEl)
            textRange = document.body.createTextRange()
            textRange.moveToElementText(tempEl)
            tempEl.parentNode.removeChild(tempEl)
        }
        textRange.text = html
        textRange.collapse(false)
        textRange.select()
    } else {
        // Chrome之类浏览器
        document.execCommand("insertText", false, html)
    }
}
```

## 捕获粘贴事件等操作方法

```javascript
// 绑定粘贴事件
document.addEventListener("paste", function (e) {});

// 阻止粘贴事件
document.addEventListener("paste", function (e) {
    e.preventDefault();
});

// 获取粘贴内容
document.addEventListener("paste", function (e) {
    var text;
    if(window.clipboardData && clipboardData.setData) {
        // IE
        text = window.clipboardData.getData('text')
    } else {
        text = (e.originalEvent || e).clipboardData.getData('text/plain')
    }
});

// 获取粘贴原始数据
document.addEventListener("paste", function (e) {
    var cbd = e.clipboardData;
    var ua = window.navigator.userAgent;

    // 如果是 Safari 直接 return
    if ( !(e.clipboardData && e.clipboardData.items) ) {
        return;
    }

    // Mac平台下Chrome49版本以下 复制Finder中的文件的Bug Hack掉
    if(cbd.items && cbd.items.length === 2 && cbd.items[0].kind === "string" && cbd.items[1].kind === "file" &&
        cbd.types && cbd.types.length === 2 && cbd.types[0] === "text/plain" && cbd.types[1] === "Files" &&
        ua.match(/Macintosh/i) && Number(ua.match(/Chrome\/(\d{2})/i)[1]) < 49){
        return;
    }

    for(var i = 0; i < cbd.items.length; i++) {
        var item = cbd.items[i];
        if (item.kind === "string") {
            item.getAsString(function (str) {
                // str 是获取到的字符串
            })
        } else if (item.kind === "file") {
            var pasteFile = item.getAsFile();
            // pasteFile就是获取到的文件
        }
    }
}, false);
```

## 横向滚动计算公式

`Math.floor((总长度-可视区域长度) * (距离顶部距离 / (总长度 - 页面可是高度)).toFixed(4)) * -1`

## 手写简单的模板引擎

**单级对象数据获取**

```javascript
var data = {
    name: 'ruoyu',
    addr: 'Hunger Valley'
};

var tpl = 'Hello, my name is  {{name}}. I am in {{addr}}.';
var reg=/{{([a-zA-Z_$][a-zA-Z0-9_.]*)}}/g;

var newStr = tpl.replace(reg,function(raw,key,offset,string){
    return data[key]||raw;
})
```

**多级对象数据获取**

```javascript
var data = {
    name: 'ruoyu',
    age: '17',
    friend: {
        name: 'hunger',
        car: {
            color: 'white'
        }
    }
}
var tpl = 'Hello, my name is  {{name}}. I am in {{age}},I have a friend {{friend.name}},he has a {{friend.car.color}} car'
var reg = /{{([a-zA-Z_$][a-zA-Z0-9_.]*)}}/g;

var newStr = tpl.replace(reg, function (raw, key, offset, string) {
    var paths = key.split('.');
    var lookup = data;
    while (paths.length > 0) {
        lookup = lookup[paths.shift()];
    }
    return lookup || raw;
})
```

## js原生获取DOM元素在父元素内的下标值

```javascript
<ul>
  <li>hello</li>
  <li>hello</li>
  <li id="mts">hello</li>
  <li>hello</li>
</ul>

var elt=document.getElementById('mts');
var index = [].indexOf.call(elt.parentNode.querySelectorAll(elt.tagName),elt);

console.log(index);
```

## 继承

```javascript
// 定义父类构造函数
var Father = function (name, age) {
	this.name = name;
	this.age = age;
};
// 定义子类构造函数
var Student = function(name, age, high) {
	// 继承父类
	Father.call(this, name, age);
	this.high = high;
};

Student.prototype.message = function() {
	console.log("name: " +　this.name + ",age: " + this.age + ",high: " + this.high);
}

new Student("xiaoming", 12, "1.6m").message(); // name: xiaoming,age: 12,high: 1.6m
```

## 绑定this指向

```javascript
var foo = {
	name: "foo",
	showName: function () {
		console.log(this.name);
	}
}
var bar = {
	name: "bar"
}
foo.showName.apply(bar); // bar
```

## 将类数组对象转换成数组对象

```javascript
function person(name, age, high) {
	console.log(arguments); // { '0': 'xiaoming', '1': 12, '2': '1.6m' }
	var arr = [].slice.apply(arguments);
	console.log(arr); // ["xiaoming", 12, "1.6m"]
}
person("xiaoming", 12, "1.6m");
```

## 背景图实现多端大小适配

```javascript
// 获取不同屏幕适配高度（适配高度 = 页面宽度 / (图片宽度 / 图片高度)）
var adapterHeight = document.body.offsetWidth / (750 / 450);
```

```css
/* 样式设置自动比例缩放*/
background-size: cover;
```

## 判断游览器是否支持touch事件

```javascript
var isSupportTouch = "ontouchend" in document ? true : false;
```

## 深入理解自定义事件绑定

```html
<form id="fo">
	<input type="text" id="msg">
	<input type="submit" value="提交">
</form>
```

```javascript
var fo = document.querySelector('#fo');
var event = new CustomEvent('newMessage', {
    detail: {
        message: 'Hello World',
        time: new Date(),
    },
    bubbles: true,
    cancelable: true,
});

fo.dispatchEvent(event);
fo.addEventListener('submit', SendMessage);

function SendMessage(e) {
    e.preventDefault();

    let msg = document.getElementById("msg").value.trim();

    if (msg && window.CustomEvent) {
        let event = new CustomEvent("newMessage", {
            detail: {
                message: msg,
                time: new Date(),
            },
            bubbles: true,
            cancelable: true
        });

        e.currentTarget.dispatchEvent(event);
    }
}

function newMessageHandler(e) {
    console.log(e.currentTarget.nodeName, e.detail.time.toLocaleString(), e.detail.message);
}
document.addEventListener("newMessage", newMessageHandler);
```

## 创建自定义事件并触发

```javascript
// 首先创建一个事件
let myEvent = new CustomEvent("userLogin", {
	detail: {
		username: "davidwalsh"
	}
});

$mask.addEventListener("userLogin", function (e) {
	console.info("Event is: ", e);
	console.info("Custom data is: ", e.detail);
})

// 触发它！
$mask.dispatchEvent(myEvent);
```


## addEventListener绑定事件触发对象

```javascript
var tap = {
  handleEvent: function() {
	alert(this.name);
  },
  name: 'tap'
};
document.getElementById('button').addEventListener('click', tap, false);
```

## instanceof原理

1、instanceof的作用是用来做检测类型：

（1）instanceof可以检测某个对象是不是另一个对象的实例；

```javascript
var Person = function() {};
var student = new Person();
console.log(student instanceof Person);  // true
```

（2）instanceof可以检测父类型；

```javascript
function Person() {};
function Student() {};
var p = new Person();
Student.prototype=p; //继承原型
var s=new Student();
console.log(s instanceof Student); //true
console.log(s instanceof Person); //true
```

但是，instanceof不适合检测一个对象本身的类型。

2、instanceof 检测一个对象A是不是另一个对象B的实例的原理：

查看对象B的prototype指向的对象是否在对象A的[[prototype]]链上。如果在，则返回true,如果不在则返回false。不过有一个特殊的情况，当对象B的prototype为null将会报错(类似于空指针异常)。

函数模拟A instanceof B：

```javascript
function _instanceof(A, B) {
	var O = B.prototype;// 取B的显示原型
	A = A.__proto__;// 取A的隐式原型
	while (true) {
		//Object.prototype.__proto__ === null
		if (A === null)
			return false;
		if (O === A)// 这里重点：当 O 严格等于 A 时，返回 true
			return true;
		A = A.__proto__;
	}
}
```

## ||和&&的妙用

```javascript
var bar = $ || 233; //如果$存在，则把$赋值给bar；如果$不存在，则把233赋值给bar
$ === undefined && (window.$ = jQuery); //如果$不存在,则把jQuery赋值给window.$；如果$存在，则不执行后面的表达式
```

## 阻止touchstart点穿方法

在ios上效果很不错，完美解决穿透点击问题，andirod上效果不好（所以有了下面的方法）。

```javascript
$mask.addEventListener('touchstart', function (e) {
	e.preventDefault();
	this.parentNode.removeChild(this);
})
```

## 原生JS实现forEach代码

```javascript
if (!Array.prototype.forEach) {
    Array.prototype.forEach = function forEach(callback, thisArg) {
        var T, k;
        if (this == null) {
            throw new TypeError("this is null or not defined");
        }
        var O = Object(this);
        var len = O.length >>> 0;
        if (typeof callback !== "function") {
            throw new TypeError(callback + " is not a function");
        }
        if (arguments.length > 1) {
            T = thisArg;
        }
        k = 0;
        while(k < len) {

            var kValue;
            if (k in O) {
                kValue = O[ k ];
                callback.call(T, kValue, k, O);
            }
            k++;
        }
    };
}
```

## 随机指定范围数字

```js
function randomNumber(n1, n2) {
    if (arguments.length === 2) {
        return Math.round(n1 + Math.random() * (n2 - n1));
    }
    else if (arguments.length === 1) {
        return Math.round(Math.random() * n1)
    }
    else {
        return Math.round(Math.random() * 255)
    }
}

randomNumber(1,3);
```

## 前端计算分配随机概率

```js
var objects = ['登山包', '旅行箱', '移动电源', '不中奖'];
var num = {
    '登山包': 0,
    '旅行箱': 0,
    '移动电源': 0,
    '不中奖': 0
}
for(var i=0; i<100000; i++){
    var randomIndex = Math.floor(objects.length * updateRandom());
    var object = objects[randomIndex];
    if(randomIndex == 0) num['登山包']++;
    if(randomIndex == 1) num['旅行箱']++;
    if(randomIndex == 2) num['移动电源']++;
    if(randomIndex == 3) num['不中奖']++;
}

console.log(num);

function updateRandom() {
    var p = Math.random()
    if (p < 0.01) return 0;
    if (p < 0.04) return 0.25
    if (p < 0.1) return 0.5;
    if (p < 1) return 0.75;
}
```

## JavaScript策略模式理解

**简单版策略模式**

```javascript
var obj = {
    "A": function (salary) {
        return salary * 4;
    },
    "B": function (salary) {
        return salary * 3;
    },
    "C": function (salary) {
        return salary * 2;
    }
};
var calculateBouns = function (level, salary) {
    return obj[level](salary);
};
console.log(calculateBouns('A', 10000)); // 40000
```

策略模式指的是定义一系列的算法，并且把它们封装起来，但是策略模式不仅仅只封装算法，我们还可以对用来封装一系列的业务规则，只要这些业务规则目标一致，我们就可以使用策略模式来封装它们；

**复杂版策略模式**

HTML

```html
<input type="text" id="text">
<input type="button" value="提交" id="submit">
```

JavaScript

```javascript
// 策略对象
var strategys = {
    isNotEmpty: function (value, errorMsg) {
        if (value === '') {
            return errorMsg;
        }
    },
    // 限制最小长度
    minLength: function (value, length, errorMsg) {
        if (value.length < length) {
            return errorMsg;
        }
    },
    // 手机号码格式
    mobileFormat: function (value, errorMsg) {
        if (!/(^1[3|5|8][0-9]{9}$)/.test(value)) {
            return errorMsg;
        }
    }
};
var Validator = function () {
    this.cache = []; // 保存效验规则
};
Validator.prototype.add = function (dom, rules) {
    var self = this;
    for (var i = 0, rule; rule = rules[i++];) {
        (function (rule) {
            var strategyAry = rule.strategy.split(":");
            console.log(strategyAry);
            var errorMsg = rule.errorMsg;
            self.cache.push(function () {
                var strategy = strategyAry.shift();
                strategyAry.unshift(dom.value);
                strategyAry.push(errorMsg);
                return strategys[strategy].apply(dom, strategyAry);
            });
        })(rule);
    }
};
Validator.prototype.start = function () {
    for (var i = 0, validatorFunc; validatorFunc = this.cache[i++];) {
        var msg = validatorFunc(); // 开始效验 并取得效验后的返回信息
        if (msg) {
            return msg;
        }
    }
};

// 代码调用
var $submit = document.getElementById("submit");
var $text = document.getElementById("text");


var validateFunc = function () {
    var validator = new Validator(); // 创建一个Validator对象
    /* 添加一些效验规则 */
    validator.add($text, [{
            strategy: 'isNotEmpty',
            errorMsg: '用户名不能为空'
        },
        {
            strategy: 'minLength:6',
            errorMsg: '用户名长度不能小于6位'
        }
    ]);
    var errorMsg = validator.start(); // 获得效验结果
    return errorMsg; // 返回效验结果
};
// 点击确定提交
$submit.onclick = function () {
    var errorMsg = validateFunc();
    if (errorMsg) {
        alert(errorMsg);
        return false;
    }
}
```

## window.location详细操作用法

**设置或获取对象指定的文件名或路径。**

```js
window.location.pathname

// 例：http://localhost:8086/topic/index?topicId=361
// 输出：`/topic/index`
```

**设置或获取整个 URL 为字符串。**

```js
window.location.href

// 例：http://localhost:8086/topic/index?topicId=361
// 输出：`http://localhost:8086/topic/index?topicId=361`
```

**设置或获取与 URL 关联的端口号码。**

```js
window.location.port

// 例：http://localhost:8086/topic/index?topicId=361
// 输出：`8086`
```

**设置或获取 URL 的协议部分。**

```js
window.location.protocol

// 例：http://localhost:8086/topic/index?topicId=361
// 输出：`http:`
```

**设置或获取 href 属性中在井号“#”后面的分段。**

```js
window.location.hash

// 例：http://localhost:8086/topic/index#12312234
// 输出：`12312234`
```

**设置或获取 location 或 URL 的 hostname 和 port 号码。**

```js
window.location.host

// 例：http://localhost:8086/topic/index?topicId=361
// 输出：`http:localhost:8086`
```

**设置或获取 href 属性中跟在问号后面的部分。**

```js
window.location.search

// 例：http://localhost:8086/topic/index?topicId=361
// 输出：`?topicId=361`
```

## 手把手实现简单的模板数据渲染

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>MVVM</title>
</head>

<body>
    <div id="app">
        <h3>姓名</h3>
        <p>{{name}}</p>
        <h3>年龄</h3>
        <div>
            <p><span>{{age}}</span></p>
        </div>
        <h3>名言</h3>
        <div>{{sign}}</div>
    </div>
    <script>
        var opt = {
            el: '#app',
            data: {
                name: '王永峰',
                age: 30,
                sign: '我就是这么一个人'
            }
        }
        // document.addEventListener('DOMContentLoaded', function () {

        // }, false)

        // 常规观察者类
        function Observer() {
            this.subNode = []
        }
        Observer.prototype = {
            addSubNode: function(node) {
                this.subNode.push(node)
            },
            update: function(newVal) {
                this.subNode.forEach(function(node) {
                    node.innerHTML = newVal
                })
            }
        }

        function Vue(opt){
            this.opt = opt;
            var root = document.querySelector(opt.el)
            this.observe(opt.data)
            this.compile(root)
        }
        Vue.prototype = {
            observe: function(data) {
                Object.keys(data).forEach(function(key) {
                    var obv = new Observer();
                    data["_" + key] = data[key];
                    Object.defineProperty(data, key, {
                        get() {
                            Observer.target && obv.addSubNode(Observer.target);
                            return data['_' + key]
                        },
                        set(newVal) {
                            obv.update(newVal)
                            data['_' + key] = newVal
                        }
                    })
                })
            },
            // 初始化页面，遍历 DOM，收集每一个key变化时，随之调整的位置，以观察者方法存放起来
            compile: function(node) {
                var that = this;
                var childNodes = node.childNodes;
                childNodes.forEach(function(child) {
                    if (!child.firstElementChild && /\{\{(.*)\}\}/.test(child.innerHTML)) {
                        let key = RegExp.$1.trim()
                        child.innerHTML = child.innerHTML.replace(new RegExp('\\{\\{\\s*' + key + '\\s*\\}\\}', 'gm'), that.opt.data[key])
                        Observer.target = child
                        that.opt.data[key]
                        Observer.target = null
                    } else if (child.firstElementChild){
                        that.compile(child)
                    }
                })
            }
        }

        var vm = new Vue(opt)

    </script>
</body>

</html>
```

## 深入拷贝对象方法

```javascript
var house = {
    name: 'payen',
    people: {
        father: true,
        mother: true
    }
}
function easyClone(obj) {
    var newObj = {};
    for (var prop in obj) {
        if (obj.hasOwnProperty(prop)) {
            newObj[prop] = obj[prop];
        }
    }
    return newObj;
}
var newHouse = easyClone(house);
```

## JavaScript精准的类型判断

```javascript
Object.prototype.toString.call([])
// "[object Array]"
Object.prototype.toString.call({})
// "[object Object]"
Object.prototype.toString.call(true)
// "[object Boolean]"
Object.prototype.toString.call('')
// "[object String]"
Object.prototype.toString.call(3)
// "[object Number]"
Object.prototype.toString.call(undefined)
// "[object Undefined]"
Object.prototype.toString.call(null)
// "[object Null]"
Object.prototype.toString.call(function(){})
// "[object Function]"
Object.prototype.toString.call(new Date())
// "[object Date]"
Object.prototype.toString.call(Math)
// "[object Math]"
Object.prototype.toString.call(JSON)
// "[object JSON]"
Object.prototype.toString.call(new RegExp())
// "[object RegExp]"
Object.prototype.toString.call(new Error())
// "[object Error]"
```

## 数组去重的四种方法

- 最基本的去重方法

思路：定义一个新数组，并存放原数组的第一个元素，然后将元素组一一和新数组的元素对比，若不同则存放在新数组中。

```javascript
function unique(arr){
　　var res = [arr[0]];
　　for(var i=1;i<arr.length;i++){
　　　　var repeat = false;
　　　　for(var j=0;j<res.length;j++){
　　　　　　if(arr[i] == res[j]){
　　　　　　　　repeat = true;
　　　　　　　　break;
　　　　　　}
　　　　}
　　　　if(!repeat){
　　　　　　res.push(arr[i]);
　　　　}
　　}
　　return res;
}
```

- 先排序在去重

思路：先将原数组排序，在与相邻的进行比较，如果不同则存入新数组

```javascript
function unique(arr){
　　var arr2 = arr.sort();
　　var res = [arr2[0]];
　　for(var i=1;i<arr2.length;i++){
　　　　if(arr2[i] !== res[res.length-1]){
　　　　　　res.push(arr2[i]);
　　　　}
　　}
　　return res;
}
```

- 利用对象的属性去重（推荐）

思路：每次取出原数组的元素，然后再对象中访问这个属性，如果存在就说明重复

```javascript
function unique(arr){
　　var res =[];
　　var json = {};
　　for(var i=0;i<arr.length;i++){
　　　　if(!json[arr[i]]){
　　　　　　res.push(arr[i]);
　　　　　　json[arr[i]] = 1;
　　　　}
　　}
　　return res;
}
```

- 利用下标查询

```javascript
function unique(arr){
　　var newArr = [arr[0]];
　　 for(var i=1;i<arr.length;i++){
　　　　if(newArr.indexOf(arr[i]) == -1){
      　　 newArr.push(arr[i]);
　　  }
    }
    return newArr;
}
```

## JS原生实现extend方法

```js
function extend(initial,replace){
    for(var item in replace){
        if(replace.hasOwnProperty(item)){
            initial[item] = replace[item]
        }
    }
    return initial
}
```

## JS判断对象属性或方法是否属于原型链

```js
[object].hasOwnProperty([key])
```

## 深度优先遍历树结构

```javascript
var data={
    key1:"str1",
    key2:{
        key3:"key3",
        key4:"key4",
        key5:{
            key6:"key6"
        }
    }
}
function treeTraversal(data) {
    function f(prefix,data) {
        var keys=Object.keys(data);
        if(!/^\s*$/.test(prefix)){
            prefix+=" ";
        }
        keys.forEach((item,index)=>{
            if (typeof data[item] == "string"){
                console.log(prefix+item+" "+data[item]);
                return prefix+item+" "+data[item];
            }else{
                prefix+=item;
                return f(prefix, data[item]);
            }
        });
    }
    f("",data);
}
treeTraversal(data);
```

## 数字千分位格式化

```javascript
function format (num) {
    let [integer,decimal]=String(num).split('.');
    let regObj=/\d{1,3}(?=(\d{3})*$)/g;
    let arr=String(integer).match(regObj);
    return arr.join(',')+(typeof decimal=="undefined"?"":'.'+decimal);
}
console.log(format(1234567890.2323));
```

## 二分查找

```js
var arr = [41, 55, 76, 87, 88, 99, 123, 432, 546, 577, 688, 786];

function twoFind(arr, wantVal, leftIndex, rightIndex) {
    if (leftIndex > rightIndex) {
        document.writeln('SORRY: 找不到 ' + wantVal + ' ！');
        return;
    }
    var minIndex = Math.floor((leftIndex + rightIndex) / 2);
    if (arr[minIndex] > wantVal) {
        twoFind(arr, wantVal, leftIndex, minIndex - 1);
    } else if (arr[minIndex] < wantVal) {
        twoFind(arr, wantVal, minIndex + 1, rightIndex);
    } else {
        document.writeln('找到了 ' + wantVal + ' ,下表为' + minIndex);
    }
}
twoFind(arr, 9, 0, arr.length - 1);
```

## 获取元素距离页面的top、left

```js
function getRec(ele) {
    var _t = document.documentElement.clientTop,
        _l = document.documentElement.clientLeft,
        rect = ele.getBoundingClientRect();
    return {
        top: rect.top - _t,
        right: rect.right - _l,
        bottom: rect.bottom - _t,
        left: rect.left - _l
    }
}
```

## JavaScript原生绑定事件和解绑事件

```js
// 绑定事件
function eventBind(obj, eventType, callBack) {
    if (obj.addEventListener) {
        obj.addEventListener(eventType, callBack, false);
    }
    else if (window.attachEvent) {
        obj.attachEvent('on' + eventType, callBack);
    }
    else {
        obj['on' + eventType] = callBack;
    }
};

// 移除事件
function moveBind(objId, eventType, callBack) {
    var obj = document.getElementById(objId);
    if (obj.removeEventListener) {
        obj.removeEventListener(eventType, callBack, false);
    }
    else if (window.detachEvent) {
        obj.detachEvent('on' + eventType, callBack);
    }
    else {
        obj['on' + eventType] = null;
    }
}
```

## 回车触发事件

```js
$("id").onkeypress = function (event) {
    event = (event) ? event : ((window.event) ? window.event : "")
    keyCode = event.keyCode ? event.keyCode : (event.which ? event.which : event.charCode);
    if (keyCode == 13) {
        $("SubmitLogin").onclick();
    }
}
```

## 对象深入拷贝方法

```js
var house = {
    name: 'payen',
    people: {
        father: true,
        mother: true
    }
}
function easyClone(obj) {
    var newObj = {};
    for (var prop in obj) {
        if (obj.hasOwnProperty(prop)) {
            newObj[prop] = obj[prop];
        }
    }
    return newObj;
}
var newHouse = easyClone(house);
```

## JavaScript阻止事件动作

```js
e.preventDefault();
```

## JavaScript阻止冒泡和捕获

```js
e.stopPropagation();
```

## call继承条件

call只能继承对象里的方法，无法继承原型链中的方法；

要继承整个对象包括原型链方法必须使用拷贝继承,方法如下:

```js
var animal = new Animal();
for(var attr in animal){
    this[attr] = animal[attr];
}
```

## createDocumentFragment()降低创建元素渲染次数

普通创建方式：

```js
for(var i=0;i<10;i++){
    var divEle = document.createElement(div);
    divEle.textContent = i;
    document.body.appendChild(divEle); //N次渲染
}
```

碎片化储存方式：

```js
var fragment = document.createDocumentFragment();
for(var i=0;i<10;i++){
    var divEle = document.createElement(div);
    divEle.textContent = i;
    fragment.appendChild(divEle);
}
document.body.appendChild(fragment); //1次渲染
```

## 通过bind()掌控this

```js
function ReplaceProcessor() {
    this._dom = {
        btnReplace : $('#ro_btnReplace'),
        btnComplete: $('#ro_btnComplete')
    };
    // Bind events
    this._dom.btnReplace.on('click', this._onReplace.bind(this));
}

ReplaceProcessor.prototype._onReplace = function(){
    // code
    this._dom.btnComplete.html("OK");
}
```

## 把对象转JSON格式输出

```
JSON.stringify(obj)
```

## 判断是否为数组对象

```
object instanceof Array

```

## JS判断显示页面是否为移动端

```js
function IsPC(){
   var userAgentInfo = navigator.userAgent;
   var Agents = new Array("Android", "iPhone", "SymbianOS", "Windows Phone", "iPad", "iPod");
   var flag = true;
   for (var v = 0; v < Agents.length; v++) {
       if (userAgentInfo.indexOf(Agents[v]) > 0) { flag = false; break; }
   }
   return flag;
}
```

## JS禁止滚轮、键盘触发滚动条滚动

```js
var keys = [37, 38, 39, 40];

function preventDefault(e) {
  e = e || window.event;
  if (e.preventDefault)
      e.preventDefault();
  e.returnValue = false;
}

function keydown(e) {
    for (var i = keys.length; i--;) {
        if (e.keyCode === keys[i]) {
            preventDefault(e);
            return;
        }
    }
}

function wheel(e) {
  preventDefault(e);
}

function disable_scroll() {
  if (window.addEventListener) {
      window.addEventListener('DOMMouseScroll', wheel, false);
  }
  window.onmousewheel = document.onmousewheel = wheel;
  document.onkeydown = keydown;
}

function enable_scroll() {
    if (window.removeEventListener) {
        window.removeEventListener('DOMMouseScroll', wheel, false);
    }
    window.onmousewheel = document.onmousewheel = document.onkeydown = null;
}

//调用方法

enable_scroll();  //允许滚动
disable_scroll();  //禁止滚动
```

## 简单的前端路由机制

```js
function Router(){
	this.routes = {};
	this.curUrl = '';

	this.route = function(path, callback){
		this.routes[path] = callback || function(){};
	};

	this.refresh = function(){
		this.curUrl = location.hash.slice(1) || '/';
		this.routes[this.curUrl]();
	};

	this.init = function(){
	    var that = this;
        $(document).ready(function(){
            that.refresh();
        })
         $(window).on('hashchange', function(){
            that.refresh();
        })
	}

}

var R = new Router();
R.init();
var res = document.getElementById('result');

 R.route('/', function() {
 	res.style.background = 'blue';
 	res.innerHTML = '这是首页';
 });
 R.route('/product', function() {
    res.style.background = 'orange';
 	res.innerHTML = '这是产品页';
 });
 R.route('/server', function() {
    res.style.background = 'black';
 	res.innerHTML = '这是服务页';
 });
 ```

## jQuery+CSS实现圆形进度条

HTML:

```html
<div class="circle">
	<div class="pie_left"><div class="left"></div></div>
	<div class="pie_right"><div class="right"></div></div>
	<div class="mask"><span>46</span>%</div>
</div>
```

CSS:

```css
.circle {
	width: 200px;
	height: 200px;
	position: absolute;
	border-radius: 50%;
	background: #0cc;
}
.pie_left, .pie_right {
	width:200px;
	height:200px;
	position: absolute;
	top: 0;left: 0;
}
.left, .right {
	width:200px;
	height:200px;
	background:#00aacc;
	border-radius: 50%;
	position: absolute;
	top: 0;
	left: 0;
}
.pie_right, .right {
	clip:rect(0,auto,auto,100px);
}
.pie_left, .left {
	clip:rect(0,100px,auto,0);
}
.mask {
	width: 150px;
	height: 150px;
	border-radius: 50%;
	left: 25px;
	top: 25px;
	background: #FFF;
	position: absolute;
	text-align: center;
	line-height: 150px;
	font-size: 20px;
	font-weight: bold;
	color: #00aacc;
}
```

Javascript:

```js
$(function() {
	$('.circle').each(function(index, el) {
		var num = $(this).find('span').text() * 3.6;
		if (num<=180) {
			$(this).find('.right').css('transform', "rotate(" + num + "deg)");
		} else {
			$(this).find('.right').css('transform', "rotate(180deg)");
			$(this).find('.left').css('transform', "rotate(" + (num - 180) + "deg)");
		};
	});
});
```

## 跨域Ajax请求时带Cookie信息

**1. 无关Cookie跨域Ajax请求**

- 客户端

以 jQuery 的 ajax 为例：
```js
$.ajax({
    url : 'http://remote.domain.com/corsrequest',
    data : data,
    dataType: 'json',
    type : 'POST',
    crossDomain: true,
    contentType: "application/json", // POST时必须
    ...
})
```
主要注意的是参数 crossDomain: true。发送Ajax时，Request header 中会包含跨域的额外信息，但不会含cookie。

- 服务器端

跨域的允许主要由服务器端控制。服务器端通过在响应的 header 中设置 Access-Control-Allow-Origin 及相关一系列参数，提供跨域访问的允许策略。相关参数的设置介绍

以Java为例：
```js
/**
* Spring Controller中的方法：
*/
    @RequestMapping(value = "/corsrequest")
    @ResponseBody
    public Map<String, Object> mainHeaderInfo(HttpServletResponse response) {
        response.setHeader("Access-Control-Allow-Origin", "*");
        ...
}
```
通过在响应 header 中设置 ‘*’ 来允许来自所有域的跨域请求访问。

```js
response.setHeader("Access-Control-Allow-Origin", "*");
```

只允许来自特定域 http://my.domain.cn:8080 的跨域访问

```js
response.setHeader("Access-Control-Allow-Origin", "http://my.domain.cn:8080");
```

较灵活的设置方式，允许所有包含 mydomain.com 的域名访问.

```js
if(request.getHeader("Origin").contains("mydomain.com")) {
    response.setHeader("Access-Control-Allow-Origin", request.getHeader("Origin"));
}
```

**2.带Cookie的跨域Ajax请求**

- 客户端

```js
$.ajax({
    url : 'http://remote.domain.com/corsrequest',
    data : data,
    dataType: 'json',
    type : 'POST',
    xhrFields: {
        withCredentials: true
    },
    crossDomain: true,
    contentType: "application/json",
    ...
```
通过设置 `withCredentials: true` ，发送Ajax时，Request header中便会带上 Cookie 信息。

- 服务器端

相应的，对于客户端的参数，服务器端也需要进行设置：

```js
/**
* Spring Controller中的方法：
*/
    @RequestMapping(value = "/corsrequest")
    @ResponseBody
    public Map<String, Object> getUserBaseInfo(HttpServletResponse response) {
        if(request.getHeader("Origin").contains("woego.cn")) {
            response.setHeader("Access-Control-Allow-Origin", request.getHeader("Origin"));
        }
        response.setHeader("Access-Control-Allow-Credentials", "true");
        ...
```
对应客户端的 `xhrFields.withCredentials: true` 参数，服务器端通过在响应 header 中设置 `Access-Control-Allow-Credentials = true` 来运行客户端携带证书式访问。通过对 Credentials 参数的设置，就可以保持跨域 Ajax 时的 Cookie。这里需要注意的是：

服务器端 `Access-Control-Allow-Credentials = true`时，参数`Access-Control-Allow-Origin` 的值不能为 '*' 。

## 原生JS把对象转化成数组遍历输出

```js
var person = {
    firstName: 'David',
    lastName: 'Walsh',
    // ...
};
Object.keys(person).forEach(function(trait) {
    console.log('Person ', trait,': ', person[trait]);
});
```

## 获取选中文字内容

```js
function getSelectText() {
    var userSelection, text;
    if (window.getSelection) {
        // Firefox support
        userSelection = window.getSelection();
    } else if (document.selection) {
        // IE Support
        userSelection = document.selection.createRange();
    }
    if (!(text = userSelection.text)) {
        var selectedText = userSelection.toString();
        text = selectedText;
    }
    return text;
}
```

## 在光标后插入内容仅支持textarea

```js
function insertAfterText(textDom, value) {
    var selectRange;
    if (document.selection) {
        // IE Support
        textDom.focus();
        selectRange = document.selection.createRange();
        selectRange.text = value;
        textDom.focus();
    }else if (textDom.selectionStart || textDom.selectionStart == '0') {
        // Firefox support
        var startPos = textDom.selectionStart;
        var endPos = textDom.selectionEnd;
        var scrollTop = textDom.scrollTop;
        textDom.value = textDom.value.substring(0, startPos) + value + textDom.value.substring(endPos, textDom.value.length);
        textDom.focus();
        textDom.selectionStart = startPos + value.length;
        textDom.selectionEnd = startPos + value.length;
        textDom.scrollTop = scrollTop;
    }
    else {
        textDom.value += value;
        textDom.focus();
    }
}
```

## 页面测试延迟毫秒封装方法

```js
var use_time = [];

use_time.push(function(){
    var str = 0;
    var obj = document.getElementById("demo");
    for(var i = 0; i < 1100; i++){
        obj.innerHTML += str + i;
    }
});

use_time.push(function(){
    var str = 0;
    var obj = document.getElementById("demo");
    for(var i = 0; i < 1100; i++){
        obj.innerHTML += str + i;
    }
});

use_time.push(function(){
    var str = 0;
    var obj = document.getElementById("demo");
    for(var i = 0; i < 400; i++){
        obj.innerHTML += str + i;
    }
});

use_time.forEach(function(val,index){
    (function(code,index){
        var start = new Date().getTime();
        code();
        var end = new Date().getTime();
        console.log(index+"用时 " + (end - start) + " 毫秒");
    })(val,index);
})
```

## JavaScript模板引擎

```html
<div class="result"></div>
<script type="template" id="template">
    <h2><a href="{{href}}">{{title}}</a></h2>
    <img src="{{imgSrc}}" alt="{{title}}">
</script>
```

```js
;(function () {
    // simulates AJAX request
    var data = [
        {
            title: "Knockout应用开发指南1",
            href: "http://www.cnblogs.com/TomXu/archive/2011/11/21/2257154.html",
            imgSrc: "http://images.cnblogs.com/cnblogs_com/TomXu/339203/o_knockout2.jpg"
        },
        {
            title: "微软ASP.NET站点部署指南",
            href: "http://www.cnblogs.com/TomXu/archive/2011/11/25/2263050.html",
            imgSrc: "http://www.cnblogs.com/images/cnblogs_com/TomXu/339203/o_vs.jpg"
        },
        {
            title: "HTML5学习笔记简明版",
            href: "http://www.cnblogs.com/TomXu/archive/2011/12/06/2277499.html",
            imgSrc: "http://images.cnblogs.com/cnblogs_com/TomXu/339203/o_LearningHtml5.png"
        }
    ],

        template = document.querySelector('#template').innerHTML,
        result = document.querySelector('.result'),
        attachTemplateToData;

    // 将模板和数据作为参数，通过数据里所有的项将值替换到模板的标签上（注意不是遍历模板标签，因为标签可能不在数据里存在）。
    attachTemplateToData = function (template, data) {
        var i = 0,
            len = data.length,
            fragment = '';

        // 遍历数据集合里的每一个项，做相应的替换
        function replace(obj) {
            var t, key, reg;

            for (key in obj) {
                reg = new RegExp('{{' + key + '}}', 'ig');
                t = (t || template).replace(reg, obj[key]);
            }

            return t;
        }

        for (; i < len; i++) {
            fragment += replace(data[i]);
        }

        return fragment;
    };

    result.innerHTML = attachTemplateToData(template, data);
})();
```
## jQuery异步加载结果处理

```js
var a1 = $.ajax({url : 'a' , data : {s : true}});

a1.done(function(result){
    //可以写它们各自的处理方法，并不冲突
});

var a2 = $.ajax({url : 'a' , data : {s : true}});
var a3 = $.ajax({url : 'a' , data : {s : true}});

$.when(a1 , a2 , a3).done(function(a1Result , a2Result , a3Result){
  //当三个ajax都完成时才会执行此方法
  //参数分别是三个ajax的返回值
});
```

## 函数节流和函数防抖方法

```html
<div id="throttle" class="demo">
    <!-- 函数节流 -->
    <div class="scroll"></div>
</div>
<div id="debounce" class="demo">
    <!-- 函数防抖 -->
    <div class="scroll"></div>
</div>

<script>
    // 函数节流
    var canRun = true;
    document.getElementById("throttle").onscroll = function () {
        if (!canRun) {
            // 判断是否已空闲，如果在执行中，则直接return
            return;
        }

        canRun = false;
        setTimeout(function () {
            console.log("函数节流");
            canRun = true;
        }, 300);
    };

    // 函数防抖
    var timer = false;
    document.getElementById("debounce").onscroll = function () {
        clearTimeout(timer); // 清除未执行的代码，重置回初始化状态

        timer = setTimeout(function () {
            console.log("函数防抖");
        }, 300);
    };
</script>
```

## JS输出今天星期几

```js
var days = ['日','一','二','三','四','五','六'];
var date = new Date();

console.log('今天是星期' + days[date.getDay()]);
```

## JavaScript原型，原型链 ? 有什么特点

每个对象都会在其内部初始化一个属性，就是prototype(原型)，当我们访问一个对象的属性时，
如果这个对象内部不存在这个属性，那么他就会去prototype里找这个属性，这个prototype又会有自己的prototype，
于是就这样一直找下去，也就是我们平时所说的原型链的概念。
关系：

```js
instance.constructor.prototype = instance.__proto__
```

特点：
JavaScript对象是通过引用来传递的，我们创建的每个新对象实体中并没有一份属于自己的原型副本。当我们修改原型时，与之相关的对象也会继承这一改变。


## 获取剪贴板图片内容

```html
// 粘贴选项框
<input type="text" id="testInput" placeholder="截屏后粘贴到输入框中" size="30" />

// JS实现代码
<script type="text/javascript">
    (function () {
        var imgReader = function (item) {
            var blob = item.getAsFile(),
                reader = new FileReader();

            reader.onload = function (e) {
                var img = new Image();
                img.src = e.target.result;
                document.body.appendChild(img);
            };

            reader.readAsDataURL(blob);
        };

        document.getElementById('testInput').addEventListener('paste', function (e) {
            var clipboardData = e.clipboardData,
                i = 0,
                items, item, types;
            console.log(clipboardData);
            if (clipboardData) {
                items = clipboardData.items;
                if (!items) {
                    return;
                }
                item = items[0];
                types = clipboardData.types || [];
                console.log(types)
                for (; i < types.length; i++) {
                    if (types[i] === 'Files') {
                        item = items[i];
                        break;
                    }
                }
                if (item && item.kind === 'file' && item.type.match(/^image\//i)) {
                    console.log(item);
                    imgReader(item);
                }
            }
        });
    })();
</script>

```

## 测试JS运行时间

```js
var start = new Date().getTime();
//运行代码行
var end = new Date().getTime();
console.log("用时 " + (end - start) + " 毫秒");
```

## JS原生API封装调用

```js
    function getElement(selector) {
        this.style = document.getElementById(selector).style;
    }

    getElement.prototype.color = function(color) {
        this.style.color = color;
        return this;
    };
    getElement.prototype.background = function(bg) {
        this.style.backgroundColor = bg;
        return this;
    };
    getElement.prototype.fontSize = function(size) {
        this.style.fontSize = size;
        return this;
    };

    //调用
    var el = new getElement('dd');
    el.color('red').background('#000').fontSize('12px');
```

## 数组方法插入HTML内容

```js
var aa = [
        '<a href="#" class="overlay" id="qrcode">dasdasd</a>',
        '<a href="#qrcode" class="article-share-qrcode" title="微信">微信</a>',
        '<span title="Share to">Share to</span>'
    ].join('');

$('#insert').append(aa);
```

## 判断一个值是否是对象

```js
function isObject(value){
  return value === Object(value);
}

isObject({}); // true
isObject(123);  // false
```

## 快速克隆一个对象

```js
var Rocker = function(name, age){
  this.name = name,
  this.age = age
}

var shock = new Rocker('Shock', 24);

shock.age = 99;

var cloneShock = Object.create(shock);

cloneShock.name // "Shock"
cloneShock.age // 99

//在不支持ES5的浏览器下，实现create方法如下：

Object.create = Object.create || function(obj){
  var F = function(){};
  F.prototype = obj;

  return new F();
}
```


## 迭代arguments

```js
function useCall() {
    [].forEach.call(arguments, function(val, key) {
        console.log(key, val)
    });
}

useCall('Bob Dylan', 'Bob Marley', 'Steve Vai');

//0 "Bob Dylan"
//1 "Bob Marley"
//2 "Steve Vai"

//将arguments转为数组
function transformToArray(arg){
  return Array.prototype.slice.call(arg);
}
```


## 数组排序

```js
[14.3, 8, 1, 64].sort(function(a, b) {
  return a - b;
});

//[1, 8, 14.3, 64]

//从大到小排序就是 b - a
```

## 简单实现合并对象

```js
function merge(root){
  for (var i = 1; i < arguments.length; i++) {
    for (var key in arguments[i]) {
      if (arguments[i].hasOwnProperty(key)) {
        root[key] = arguments[i][key];
      }
    }
  }
  return root;
}

var merged = merge(
  {name:'Shock'},
  {city:'Shenzhen'}
)//{name:'Shock',city:'Shenzhen'}
```

## 使用break + labels退出循环

```js
function findNumber(arr){
  loop:{
    for (var i = 0; i < arr.length; i++) {
      if(arr[i]%2 == 0){
        break loop;//表示退出loop区块
      }
    }
    console.log(arr);//这句代码是不会执行的，如果上面只是break，for循环之后的代码还是会执行
  }
}

findNumber([1,3,5,6]);
```

 ## 巧用||和&&快捷判断处理方法

```js
var bar = $ || 233;
//如果$存在，则把$赋值给bar；如果$不存在，则把233赋值给bar

$ === undefined && (window.$ =  jQuery);
//如果$不存在,则把jQuery赋值给window.$；如果$存在，则不执行后面的表达式
```

 ## 原生JS拖拽效果

 ```javascript
 <div id="main"> </div><script>
/*1：拖拽的时候有文字选中会有问题；
          原因：这是浏览器的默认拖拽文字的行为
          解决方案：标准浏览器下：阻止默认行为,在onmousedown结尾加上return false即可
           ie8及其以下版本：设置全局捕获，方法如下设置全局捕获setCapture最后释放releaseCapture
*/

var oDiv = document.getElementById("main");
oDiv.onmousedown = function(ev) {

    var ev = ev || event;
    var disX = ev.clientX - this.offsetLeft;
    var disY = ev.clientY - this.offsetTop;

    if (oDiv.setCapture) {
        oDiv.setCapture();
    }
    document.onmousemove = function(ev) {
        //这里为什么使用document，是因为快速拖拽的话会鼠标丢失，
        var ev = ev || event;
        oDiv.style.left = ev.clientX - disX + "px";
        oDiv.style.top = ev.clientY - disY + "px";
    };

    document.onmouseup = function(ev) {
        document.onmousemove = document.onmouseup = null;
        //为何不用oDiv.onmouseup是因为被挡住之后会无视掉遮挡的元素
        if (oDiv.releaseCapture) {

            oDiv.releaseCapture();
        }
    };
    return false;
}

```

Firefox可以使用filter+svg实现blur效果，url参数中原本使用的是svg路径#blur，svg、css、js都在CDN中，但发现这个svg在FF中不工作，图片显示为纯黑色，ORZ...于是想到了用base64来转码这个svg文件：

```html
<svg>
    <filter id="blur">
        <feGaussianBlur stdDeviation="25" />
    </filter>
</svg>
```

在线转码：http://b64.io/

转好后还是老问题，有点莫名，g了下发现，svg tag需要增加文档类型：

```html
<svg version="1.1" xmlns="http://www.w3.org/2000/svg">
    <filter id="blur">
        <feGaussianBlur stdDeviation="25" />
    </filter>
</svg>
```

## 减少页面的重绘

减少页面重绘虽然本质不是JS本身的优化，但是其往往是由JS引起的，而重绘的情况往往是严重影响页面性能的，所以完全有必要拿出来，我们看下面例子：
```html
<div id="demo"></div>
<input type="button" value="效率低" onclick="func1()" />
<input type="button" value="效率高" onclick="func2()" />
```

```js
var str = "<div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div><div>这是一个测试字符串</div>";
//效率低的

function func1(){
    var obj = document.getElementById("demo");
    var start = new Date().getTime();
    for(var i = 0; i < 100; i++){
        obj.innerHTML += str + i;
    }
    var end = new Date().getTime();
    alert("用时 " + (end - start) + " 毫秒");
}

//效率高的
function func2(){
    var obj = document.getElementById("demo");
    var start = new Date().getTime();
    var arr = [];
    for(var i = 0; i < 100; i++){
        arr[i] = str + i;
    }
    obj.innerHTML = arr.join("");
    var end = new Date().getTime();
    alert("用时 " + (end - start) + " 毫秒");
}
```

在例子中，我只是用了100次的循环，因为如果用10000次循环的话，浏览器基本上就卡住不动了，但是即使是100次的循环，我们看看下面的执行结果。

## JS构建简单的路由系统

```javascript
(function() {
  var util = {
    //获取路由的路径和详细参数
    getParamsUrl:function(){
      var hashDeatail = location.hash.split("?"),
        hashName = hashDeatail[0].split("#")[1],//路由地址
        params = hashDeatail[1] ? hashDeatail[1].split("&") : [],//参数内容
        query = {};
      for(var i = 0;i<params.length ; i++){
        var item = params[i].split("=");
        query[item[0]] = item[1]
      }
      return     {
        path:hashName,
        query:query
      }
    }
  };
  function spaRouters(){
    this.routers = {};//保存注册的所有路由
    this.beforeFun = null;//切换前
    this.afterFun = null;
  }
  spaRouters.prototype={
    init:function(){
      var self = this;
      //页面加载匹配路由
      window.addEventListener('load',function(){
        self.urlChange()
      });
      //路由切换
      window.addEventListener('hashchange',function(){
        self.urlChange()
      });
      //异步引入js通过回调传递参数
      window.SPA_RESOLVE_INIT = null;
    },
    refresh:function(currentHash){
      var self = this;
      if(self.beforeFun){
        self.beforeFun({
          to:{
            path:currentHash.path,
            query:currentHash.query
          },
          next:function(){
            self.routers[currentHash.path].callback.call(self,currentHash)
          }
        })
      }else{
        self.routers[currentHash.path].callback.call(self,currentHash)
      }
    },
    //路由处理
    urlChange:function(){
      var currentHash = util.getParamsUrl();
      if(this.routers[currentHash.path]){
        this.refresh(currentHash)
      }else{
        //不存在的地址重定向到首页
        location.hash = '/index'
      }
    },
    //单层路由注册
    map:function(path,callback){
      path = path.replace(/\s*/g,"");//过滤空格
      if(callback && Object.prototype.toString.call(callback) === '[object Function]' ){
        this.routers[path] ={
          callback:callback,//回调
          fn:null //存储异步文件状态
        }
      }else{
        console.trace('注册'+path+'地址需要提供正确的的注册回调')
      }
    },
    //切换之前一些处理
    beforeEach:function(callback){
      if(Object.prototype.toString.call(callback) === '[object Function]'){
        this.beforeFun = callback;
      }else{
        console.trace('路由切换前钩子函数不正确')
      }
    },
    //切换成功之后
    afterEach:function(callback){
      if(Object.prototype.toString.call(callback) === '[object Function]'){
        this.afterFun = callback;
      }else{
        console.trace('路由切换后回调函数不正确')
      }
    },
    //路由异步懒加载js文件
    asyncFun:function(file,transition){
      var self = this;
      if(self.routers[transition.path].fn){
        self.afterFun && self.afterFun(transition);
        self.routers[transition.path].fn(transition)
      }else{
        console.log("开始异步下载js文件"+file);
        var _body= document.getElementsByTagName('body')[0];
        var scriptEle= document.createElement('script');
        scriptEle.type= 'text/javascript';
        scriptEle.src= file;
        scriptEle.async = true;
        SPA_RESOLVE_INIT = null;
        scriptEle.onload= function(){
          console.log('下载'+file+'完成');
          self.afterFun && self.afterFun(transition);
          self.routers[transition.path].fn = SPA_RESOLVE_INIT;
          self.routers[transition.path].fn(transition)
        };
        _body.appendChild(scriptEle);
      }
    },
    //同步操作
    syncFun:function(callback,transition){
      this.afterFun && this.afterFun(transition);
      callback && callback(transition)
    }

  };
  //注册到window全局
  window.spaRouters = new spaRouters();
})();

spaRouters.map('/index',function(transition){
    spaRouters.asyncFun('js/index.js',transition)
})
spaRouters.map('/list',function(transition){
    spaRouters.asyncFun('js/list.js',transition)
})
spaRouters.map('/detail',function(transition){
    spaRouters.asyncFun('js/detail.js',transition)
})
spaRouters.map('/detail2',function(transition){
    spaRouters.syncFun(function(transition){
        document.getElementById("content").innerHTML = '<p style="color:#DD8C6F;">当前同步渲染详情页' + JSON.stringify(transition) +'</p>'
    },transition)
})
spaRouters.beforeEach(function(transition){
    console.log('切换之前dosomething')
    setTimeout(function(){
        //模拟切换之前延迟，比如说做个异步登录信息验证
        transition.next()
    },100)
})
spaRouters.afterEach(function(transition){
    console.log("切换之后dosomething")
})

spaRouters.init();
```

## Js/Jquery获取iframe中的元素

- js

**在父窗口中获取iframe中的元素**
方法1
格式：
```js
window.frames["iframe的name值"].document.getElementById("iframe中控件的ID").click();
```

实例：
```js
.frames["ifm"].document.getElementById("btnOk").click();
```

格式：
```js
var obj=document.getElementById("iframe的name").contentWindow;
var ifmObj=obj.document.getElementById("iframe中控件的ID");
ifmObj.click();
```
实例：
```js
var obj=document.getElementById("ifm").contentWindow;
var ifmObj=obj.document.getElementById("btnOk");
ifmObj.click();
```

**在iframe中获取父窗口的元素**

格式：
```js
window.parent.document.getElementById("父窗口的元素ID").click();
```
实例：
```js
window.parent.document.getElementById("btnOk").click();
```

- jquery

**在父窗口中获取iframe中的元素**

方法1

格式：
```js
$("#iframe的ID").contents().find("#iframe中的控件ID").click();//jquery
```
实例：
```js
$("#ifm").contents().find("#btnOk").click();//jquery 方法1
```
方法2

格式：
```js
$("#iframe中的控件ID",document.frames("frame的name").document).click();//jquery 方法2
```
实例：
```js
$("#btnOk",document.frames("ifm").document).click();//jquery 方法2
```
**在iframe中获取父窗口的元素**

格式：
```js
$('#父窗口中的元素ID', parent.document).click();
```
实例：
```js
$('#btnOk', parent.document).click();
```