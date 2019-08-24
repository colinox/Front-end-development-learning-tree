<!-- TOC -->

- [Vue创建全局组件使用Vue.use()载入](#vue创建全局组件使用vueuse载入)
- [vue实现异步组件](#vue实现异步组件)
- [设置Nuxt所有公共路径方法](#设置nuxt所有公共路径方法)
- [Nuxt CSS文件抽离成文件方法](#nuxt-css文件抽离成文件方法)
- [Vue / keep-alive缓存页面](#vue--keep-alive缓存页面)
- [Vue监听定义属性和属性修改变化](#vue监听定义属性和属性修改变化)
- [Vue分离式处理项目代码](#vue分离式处理项目代码)
- [Vue组件v-model绑定快速修改参数](#vue组件v-model绑定快速修改参数)
- [Vue组件非绑定传值](#vue组件非绑定传值)
- [Vue this.$forceUpdate()强制刷新渲染页面](#vue-thisforceupdate强制刷新渲染页面)
- [Vue子组件快速修改父组件参数](#vue子组件快速修改父组件参数)
- [Vue Router路由懒加载配置](#vue-router路由懒加载配置)
- [Nuxt使用pm2启动配置](#nuxt使用pm2启动配置)
- [NUXT添加插件](#nuxt添加插件)
- [NUXT中间件使用方法](#nuxt中间件使用方法)
- [NUXT自定义布局文件](#nuxt自定义布局文件)
- [NUXT全局CSS设置方法](#nuxt全局css设置方法)
- [Vue路由监听方法大全](#vue路由监听方法大全)
- [v-on的修饰符](#v-on的修饰符)
- [vue编程式路由实现新窗口打开](#vue编程式路由实现新窗口打开)
- [动态监听vuex的state变化](#动态监听vuex的state变化)
- [Vue获取DOM元素方法](#vue获取dom元素方法)
- [Vue v-cloak解决刷新或者加载出现闪烁（显示变量）](#vue-v-cloak解决刷新或者加载出现闪烁显示变量)
- [Vue通过计算函数改变Data内容](#vue通过计算函数改变data内容)
- [Vue监听路由变化方法](#vue监听路由变化方法)
- [Vue监听数组中对象属性的变化](#vue监听数组中对象属性的变化)
- [Vuex学习笔记](#vuex学习笔记)

<!-- /TOC -->

## Vue创建全局组件使用Vue.use()载入

loading.js

```js
import turns from './turns.vue'

const loading = {
    install: function (Vue) {
        Vue.component('turns', turns)
    }
}

export default loading;
```

main.js

```js
import Vue from 'vue';
import loading from './lib/loading';

Vue.use(loading);
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

## 设置Nuxt所有公共路径方法

在nuxt.config.js下的build里添加

```js
build: {
    publicPath: 'http://nickfu.com/_nuxt/'
}
```

## Nuxt CSS文件抽离成文件方法

在nuxt.config.js下的build里添加

```js
build: {
    extractCSS: { allChunks: true },
}
```

## Vue / keep-alive缓存页面

把需要缓存的组件name添加到include里,子组件添加缓存必须在父组件也存在缓存的情况才生效。当页面被缓存后将不执行vue生命周期方法。

- 利用include、exclude属性

```html
<keep-alive include="bookLists,bookLists">
    <router-view></router-view>
</keep-alive>
<keep-alive exclude="indexLists">
    <router-view></router-view>
</keep-alive>
```

include属性表示只有name属性为bookLists，bookLists的组件会被缓存，（注意是组件的名字，不是路由的名字）其它组件不会被缓存exclude属性表示除了name属性为indexLists的组件不会被缓存，其它组件都会被缓存

- 利用meta属性

```js
export default[
    {
        path:'/',
        name:'home',
        components:Home,
        meta:{
            keepAlive:true //需要被缓存的组件
        }
    },
    {
        path:'/book',
        name:'book',
        components:Book,
        meta:{
            keepAlive:false //不需要被缓存的组件
        }
    }
]
```

```html
<!--这里是会被缓存的组件-->
<keep-alive>
    <router-view v-if="this.$route.meat.keepAlive"></router-view>
</keep-alive>
<!--这里是不会被缓存的组件-->
<keep-alive v-if="!this.$router.meta.keepAlive"></keep-alive>
```

## Vue监听定义属性和属性修改变化

```js
export default {
    data() {
        dog: ""
    },
    watch: {
        dog: {
            handler(newVal, oldVal) {
                console.log(`Dog changed: ${newVal}`);
            },
            immediate: true
        }
    }
}
```

## Vue分离式处理项目代码

user.js：

```js
export default {
  data () {
    return {
      userInfo: null
    }
  },
  methods: {
    getUserInfo () {
      // 这里通过 ajax 获取用户信息后，赋值给 this.userInfo，以下为伪代码
      $.ajax('/user/info', (data) => {
        this.userInfo = data;
      });
    },
    setUserInfo (){
        this.userInfo = '我的信息';
    }
  },
  mounted () {
    this.getUserInfo();
  }
}
```

app.vue：

```html
<script>
import userInfo from '@plugins/user.js'

export default {
    mixins: [userInfo],
    data () {
      return {

      }
    },
    mounted () {
        this.setUserInfo();
    }
}
</script>
```

## Vue组件v-model绑定快速修改参数

app.vue

```html
<template>
    <div id='app'>
        <Header v-model="title" />
    </div>
</template>

<script>
import Header from '@components/header';

export default {
    data () {
        return {
            title: '这是一个标题'
        }
    },
    components: {
        Header
    }
}
</script>
```

Header.vue

```html
<template>
    <div id='header'>
        <h1>{{value}}</h1>
        <button @click="changeTitle">改变title</button>
    </div>
</template>
<script>

export default {
    data () {
        return {

        }
    },
    props: {
        'value': {
            type: String,
            default: ''
        }
    },
    methods: {
        changeTitle(){
            this.$emit('input','这是一个新标题');
        }
    }
}
```

## Vue组件非绑定传值

app.vue

```html
<template>
<div id='app'>
    <Header />
</div>
</template>
<script>
import Header from '@components/header';

export default {
    provide(){
        return {
            name: this.title
        }
    }
    data(){
        return {
            title: '这个标题'
        }
    }
}
```

header.vue

```js
export default {
    inject: ['name'],
    data () {
        return {

        }
    },
    mounted() {
        console.log(this.name);  // 这个标题
    }
}
```

## Vue this.$forceUpdate()强制刷新渲染页面

于一些嵌套特别深的数据，导致数据更新了，但是页面却没有重新渲染。我遇到的一个情况是，v-for遍历数据渲染，当方法中处理相应数组数据时，数组改变了，但是页面却没有重新渲染。

解决方法：运用 `this.$forceUpdate()` 强制刷新，解决v-for更新数据不重新渲染页面。

官方解释：迫使 Vue 实例重新渲染。注意它仅仅影响实例本身和插入插槽内容的子组件，而不是所有子组件。

## Vue子组件快速修改父组件参数

父组件

```html
<template>
    <div>
        <child-com :value.sync="text"></child-com>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                text:"父组件的值",
            }
        },
    }
</script>
```

子组件

```html
<template>
    <div @click="post"></div>
</template>

<script>
    export default{
        methods:{
            post(){
                this.$emit('update:value',"子组件的值")
            }
        }
    }
</script>
```

## Vue Router路由懒加载配置

```js
export default new Router({
    routes: [
        // 第一种方法
        {
            path: "/",
            name: "home",
            component: r => require.ensure([], () => r(require('./view/Home.vue')), 'home')
        },
        // 第二种方法
        {
            path: "/about",
            name: "about",
            component: resolve => require(['./view/About.vue'], resolve)
        }
        // 第三种方法(此方法需要webpack配置dynamic-import-webpack)
        {
            path: "/about",
            name: "about",
            component: () => import('./views/About.vue')
        }
    ]
});
```

## Nuxt使用pm2启动配置

```
"scripts": {
    "dev": "cross-env NODE_ENV=development nodemon server/index.js --watch server",
    "build": "nuxt build",
    "open": "nuxt build && pm2 start npm --name 'SanjiekeNuxt' -- run start",
    "reload": "nuxt build && pm2 reload SanjiekeNuxt",
    "start": "PORT=3002 nuxt start",
    "generate": "nuxt generate"
}
```

## NUXT添加插件

**1.在plugins目录下添加插件文件**

vue-notifications.js

```javascript
import Vue from 'vue'
import VueNotifications from 'vue-notifications'
import miniToastr from 'mini-toastr'

const toast = function ({ title, message, type, timeout, cb }) {
  return miniToastr[type](message, title, timeout, cb)
}

const options = {
  success: toast,
  error: toast,
  info: toast,
  warn: toast
}

Vue.use(VueNotifications, options)
```

**2.nuxt.config.js文件中添加插件配置**

```javascript
export default {
    plugins: [
        { src: '~/plugins/vue-notifications.js', ssr: false }
    ]
}
```

## NUXT中间件使用方法

**1.在middleware目录下添加中间件文件**

user-agent.js

```javascript
export default function (context) {
    context.userAgent = process.server ? context.req.headers['user-agent'] : navigator.userAgent
}
```

**2.nuxt.config.js文件中添加中间件配置**

```javascript
export default {
    router: {
        middleware: ['user-agent']
    }
}
```

**3.在路由文件中调用该方法**

```javascript
export default {
    asyncData({ store, route, userAgent }) {
        return {
            userAgent
        }
    }
}
```

## NUXT自定义布局文件

在路由文件中声明布局文件：

```javascript
export default {
    layout: 'dark'
}
```


## NUXT全局CSS设置方法

在nuxt.config.js配置文件中添加

```javascript
export default {
    css: [
        '~/css/main.css'
    ],
}
```

## Vue路由监听方法大全

**通过watch监听**

```javascript
watch:{
  $route(to,from){
	console.log(to.path);
  }
}
```

或

```javascript
watch: {
  $route: {
	handler: function(val, oldVal){
	  console.log(val);
	},
	// 深度观察监听
	deep: true
  }
}
```

或

```javascript
watch: {
  '$route':'getPath'
},
methods: {
  getPath(){
	console.log(this.$route.path);
  }
}
```

**key是用来阻止“复用”的**

Vue 为你提供了一种方式来声明“这两个元素是完全独立的——不要复用它们”。只需添加一个具有唯一值的 key 属性即可(Vue文档原话)

```html
<router-view :key="key"></router-view>
```

```javascript
computed: {
  key() {
	return this.$route.name !== undefined? this.$route.name +new Date(): this.$route +new Date()
  }
}
```

使用computed属性和Date()可以保证每一次的key都是不同的，这样就可以如愿刷新数据了。


**通过 vue-router 的钩子函数 beforeRouteEnter  beforeRouteUpdate  beforeRouteLeave**

```javascript
beforeRouteEnter (to, from, next) {
	// 在渲染该组件的对应路由被 confirm 前调用
	// 不！能！获取组件实例 `this`
	// 因为当钩子执行前，组件实例还没被创建
},
beforeRouteUpdate (to, from, next) {
	// 在当前路由改变，但是该组件被复用时调用
	// 举例来说，对于一个带有动态参数的路径 /foo/:id，在 /foo/1 和 /foo/2 之间跳转的时候，
	// 由于会渲染同样的 Foo 组件，因此组件实例会被复用。而这个钩子就会在这个情况下被调用。
	// 可以访问组件实例 `this`
},
beforeRouteLeave (to, from, next) {
	// 导航离开该组件的对应路由时调用
	// 可以访问组件实例 `this`
},
```

## v-on的修饰符

```html
<!-- 触发点击 -->
<button @click="doThis"></button>
<!-- 停止冒泡 -->
<button @click.stop="doThis"></button>
<!-- 阻止默认行为 -->
<button @click.prevent="doThis"></button>
<!-- 阻止默认行为，没有表达式 -->
<form @submit.prevent></form>
<!--  串联修饰符 -->
<button @click.stop.prevent="doThis"></button>
<!-- 键修饰符，键别名 -->
<input @keyup.enter="onEnter">
<!-- 键修饰符，键代码 -->
<input @keyup.13="onEnter">
<!-- 点击回调只会触发一次 -->
<button v-on:click.once="doThis"></button>
```

## vue编程式路由实现新窗口打开

- <router-link>标签实现新窗口打开：

官方文档中说 v-link 指令被 `<router-link>` 组件指令替代，且 `<router-link>` 不支持 target="_blank" 属性，如果需要打开一个新窗口必须要用`<a>`标签，但事实上vue2版本的 `<router-link>` 是支持  target="_blank" 属性的(tag="a")，示例如下：

```html
<router-link tag="a" target="_blank" :to="{name:'searchGoods',params:{catId:0},query:{keywords:'手机'}}">热门好货</router-link>
```
注：只有tag="a"模式下  target="_blank" 属性才会生效。

- 编程式导航：

有些时候需要在单击事件或者在函数中实现页面跳转，那么可以借助router的示例方法，通过编写代码实现。我们常用的是 $router.push 和 $router.go ,但是vue2.0以后，这种方式就不支持新窗口打开的属性了。这两种平常用的都比较多，这里就不再赘述。百度了下，找到了使用 $router.resolve 这种方法能够实现新窗口打开，示例代码如下：

```javascript
let routeData = this.$router.resolve({
   name: "searchGoods",
   query: params,
   params:{catId:params.catId}
});
window.open(routeData.href, '_blank');
```

## 动态监听vuex的state变化

vuex

```javascript
const state={
  wifiList:[]
};

const getters={
    getWiFiList: state => {
        return state.wifiList;
    }
};


export default new Vuex.Store({
    state,
    getters,
    mutations,
    actions
});
```

vue

```javascript
import {mapGetters,mapState} from "vuex";

computed:{
    ...mapGetters(['getWiFiList'])
},
watch: {
    getWiFiList: function(value) {
        console.log("改变",value);
    }
}
```

## Vue获取DOM元素方法

template:

```html
<input type="text" ref="inputText">
```

JavaScript

```javascript
this.$refs.inputText;   // 获取inputText的DOM节点
```

## Vue v-cloak解决刷新或者加载出现闪烁（显示变量）

在使用vue绑定数据的时候，渲染页面时会出现变量闪烁，例如

```html
<div class="#app">
    <p>{{value.name}}</p>
</div>
```

在加载的时候会看到

```js
{{value.name}}
```

在页面出现，过了几秒之后才会渲染数据，在vue中有个指令可以解决这个问题，v-cloak
那么，v-cloak要放在什么位置呢，是不是每个需要渲染数据的标签都要添加这个指令，经过试验发现，v-cloak并不需要添加到每个标签，只要在el挂载的标签上添加就可以，

```html
<div class="#app" v-cloak>
    <p>{{value.name}}</p>
</div>
```

而且，在css里面要添加

```css
[v-cloak] {
    display: none;
}
```

这样就可以防止页面闪烁了。
但是有的时候会不起作用，可能的原因有二：

1、v-cloak的display属性被层级更高的给覆盖掉了，所以要提高层级

```css
[v-cloak] {
    display: none !important;
}
```

2、样式放在了@import引入的css文件中

v-cloak的这个样式放在@import 引入的css文件中不起作用，可以放在link引入的css文件里或者内联样式中

## Vue通过计算函数改变Data内容

```html
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{name}}</h2>
    <h3>{{full}}</h3>
    <button @click="infoEdit">改变</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      name: 'colin'
    }
  },
  computed: {
    full: {
      get(){
        return this.msg + this.name;
      },
      set(newValue){
        var value = newValue.split(' ');
        this.msg = value[0] + value[1];
        this.name = value[2];
      }
    }
  },
  methods: {
    infoEdit:function(){
      this.full = "I Love You"
    }
  }
}
</script>
```

## Vue监听路由变化方法

**第一种**
```
beforeRouteUpdate (to, from, next) { //路由变化
    next();
}
```

**第二种**
```
watch: {
    '$route' (to, from) {
        console.log("当前路由路径",this.$route.path);
    }
}
```

## Vue监听数组中对象属性的变化

```javascript
data () {
  return {
    phone: [
      {
        name: '工作',
        telNum: ''
      }
    ]
  }
},
watch: {
  phone: {
    handler: function (newVal) {
      console.log(newVal)
    },
    deep: true
  }
}
```

## Vuex学习笔记

store.js

```javascript
const state = {
  name: '',
  age: 24
};

const mutations = {
    // 显式的更改state里的数据
    change:function(state,a){
        //  state.age++;
        console.log(state.age += a);
    },
    changeAsync:function(state,a){
        console.log(state.num += a);
    }
};

const getters = {
    getAge:function(state){
        return state.age;
    }
};

const actions = {
　　 // 设置延时
    add:function(context,value){
        setTimeout(function(){
　　　　　    // 提交事件
            context.commit('changeAsync',value);
        },1000)

    }
}

export default new Vuex.Store({
  getters,
  state,
  mutations
})
```

**state获取方法**

```
this.$store.state.age
```

**mutations调用方法**

```
this.$store.commit('change',10)
```

**getters调用方法**

```
this.$store.getters.getAge
```

**actions调用方法**

```
this.$store.dispatch('add', 5);
```

-----------------------

**vue页面内调用方法**

引入方法：

```javascript
import {mapState,mapActions,mapMutations,mapGetters} from 'vuex'
```

- mapState（状态）
- mapMutations（方法）
- mapGetters（计算状态）
- mapActions（异步方法）

使用方法：

```javascript
export default {
    computed: {
        ...mapState(['...']),
        ...mapGetters(['...'])
    },
    methods: {
        ...mapMutations(['...']),
        ...mapActions(['...'])
    }
}
```