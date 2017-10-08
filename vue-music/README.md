# vue-music

> Vue.js 打造高级实战——音乐 App

## 项目树
```
.
├── README.md
├── build
│   ├── build.js
│   ├── check-versions.js
│   ├── dev-client.js
│   ├── dev-server.js
│   ├── utils.js
│   ├── vue-loader.conf.js
│   ├── webpack.base.conf.js
│   ├── webpack.dev.conf.js
│   └── webpack.prod.conf.js
├── config
│   ├── dev.env.js
│   ├── index.js
│   └── prod.env.js
├── index.html
├── package.json
├── prod.server.js
├── src
│   ├── App.vue
│   ├── api
│   │   ├── config.js
│   │   ├── rank.js
│   │   ├── recommend.js
│   │   ├── search.js
│   │   ├── singer.js
│   │   └── song.js
│   ├── base
│   │   ├── confirm
│   │   │   └── confirm.vue
│   │   ├── listview
│   │   │   └── listview.vue
│   │   ├── loading
│   │   │   ├── loading.gif
│   │   │   └── loading.vue
│   │   ├── no-result
│   │   │   ├── no-result.vue
│   │   │   ├── no-result@2x.png
│   │   │   └── no-result@3x.png
│   │   ├── progress-bar
│   │   │   └── progress-bar.vue
│   │   ├── progress-circle
│   │   │   └── progress-circle.vue
│   │   ├── scroll
│   │   │   └── scroll.vue
│   │   ├── search-box
│   │   │   └── search-box.vue
│   │   ├── search-list
│   │   │   └── search-list.vue
│   │   ├── slider
│   │   │   └── slider.vue
│   │   ├── song-list
│   │   │   ├── first@2x.png
│   │   │   ├── first@3x.png
│   │   │   ├── second@2x.png
│   │   │   ├── second@3x.png
│   │   │   ├── song-list.vue
│   │   │   ├── third@2x.png
│   │   │   └── third@3x.png
│   │   ├── switches
│   │   │   └── switches.vue
│   │   └── top-tip
│   │       └── top-tip.vue
│   ├── common
│   │   ├── fonts
│   │   │   ├── music-icon.eot
│   │   │   ├── music-icon.svg
│   │   │   ├── music-icon.ttf
│   │   │   └── music-icon.woff
│   │   ├── image
│   │   │   └── default.png
│   │   ├── js
│   │   │   ├── cache.js
│   │   │   ├── config.js
│   │   │   ├── dom.js
│   │   │   ├── jsonp.js
│   │   │   ├── mixin.js
│   │   │   ├── singer.js
│   │   │   ├── song.js
│   │   │   └── util.js
│   │   └── stylus
│   │       ├── base.styl
│   │       ├── icon.styl
│   │       ├── index.styl
│   │       ├── mixin.styl
│   │       ├── reset.styl
│   │       └── variable.styl
│   ├── components
│   │   ├── add-song
│   │   │   └── add-song.vue
│   │   ├── disc
│   │   │   └── disc.vue
│   │   ├── m-header
│   │   │   ├── logo@2x.png
│   │   │   ├── logo@3x.png
│   │   │   └── m-header.vue
│   │   ├── music-list
│   │   │   └── music-list.vue
│   │   ├── player
│   │   │   └── player.vue
│   │   ├── playlist
│   │   │   └── playlist.vue
│   │   ├── rank
│   │   │   └── rank.vue
│   │   ├── recommend
│   │   │   └── recommend.vue
│   │   ├── search
│   │   │   └── search.vue
│   │   ├── singer
│   │   │   └── singer.vue
│   │   ├── singer-detail
│   │   │   └── singer-detail.vue
│   │   ├── suggest
│   │   │   └── suggest.vue
│   │   ├── tab
│   │   │   └── tab.vue
│   │   ├── top-list
│   │   │   └── top-list.vue
│   │   └── user-center
│   │       └── user-center.vue
│   ├── main.js
│   ├── router
│   │   └── index.js
│   └── store
│       ├── actions.js
│       ├── getters.js
│       ├── index.js
│       ├── mutation-types.js
│       ├── mutations.js
│       └── state.js
└── static
    ├── 1.png
    ├── 2.png
    ├── 3.png
    ├── 4.png
    └── 5.png

```

# 技术栈

Vue2：采用最新Vue2的语法

Vuex：实现不同组件之间的状态共享

vue-router：单页应用路由管理必备

axios：发起http请求

Less：css预处理语言

IScroll：模拟原生app的列表滚动效果(ListView)

Flex：flex弹性布局，简单适配手机、PC端

Express(上线版本是Koa2)：因为vue-cli是用的Express做服务器，所以开源的开发版本是Express，自己生产环境用的是Koa2。

Webpack：自动化构建工具，大部分配置vue-cli脚手架已经弄好了，很方便。

ES6：采用ES6语法，这是趋势。

IScroll：模拟原生app的列表滚动效果(ListView)

jsonp：跨域请求数据

localStorage(HTML5)：本地存储，保存用户个性化设置。

CSS3：CSS3动画及样式。

## 项目截图

<!-- ![image](https://github.com/songhaoreact/vue-music/blob/master/static/1.png)

![image](https://github.com/songhaoreact/vue-music/blob/master/static/2.png)

![image](https://github.com/songhaoreact/vue-music/blob/master/static/3.png)

![image](https://github.com/songhaoreact/vue-music/blob/master/static/4.png)

![image](https://github.com/songhaoreact/vue-music/blob/master/static/5.png) -->

## 遇到的问题

目前已经实现了播放器的核心功能，如歌曲列表、歌手列表、搜索音乐、搜索歌手、歌曲快速入口、歌手详情、歌曲详情、歌词滚动、播放歌曲滚动、播放方式设置、个人用户设置、添加好友、歌曲排行、歌手排行、歌曲播放、歌曲皮肤切换、注销、切换用户等等。后期会考虑增加更多功能。

1.异步编程：JS是单线程，异步编程尤为重要。当我们向后端请求数据，是异步的，如果没有处理好相关的异步操作，是会有各种问题的。JS可以利用setTimeout、回调、Generator、Promise、Async。 定时这种方式太麻烦，还是不推荐；回调层次多了，有回调地狱，代码维护性很差；Generator需要手动去执行，当然可以使用类似co的模块。相比之下Promise和Async是比较理想的。 
2.尽量在vue中少操作dom元素，在此项目中只有在不得已的情况下才会操作dom
3.各组件结构的设计：一开始大纲没设计好，后面想修改涉及面会很广。
4.过渡动画让交互更有趣，但是有的还是耗性能的，有设备差异，没用好会造成卡顿。


### 安装与运行

```
<!-- git clone https://github.com/songhaoreact/vue-music.git -->

cd vue-music

npm install

npm run dev //服务端运行 访问 http://localhost:8080

npm run build 项目打包 

感兴趣的童鞋可以来个star

