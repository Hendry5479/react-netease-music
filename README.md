# React实战之云音乐项目

> 如果觉得不错，或者对你有帮助，点一个star~

### 1.1. 项目简介
使用React编写的云音乐Web项目，接口来源于[网易云音乐 NodeJS 版 API](https://binaryify.github.io/NeteaseCloudMusicApi/#/)，自己已经做了部署
感谢王红元老师的React课程，让我受益匪浅。
目前完成“发现音乐”和“我的音乐”模块的部分功能，计划继续完善项目功能。
效果一览：http://121.36.81.230:80 (域名正在备案中...)
**推荐页面**：

![推荐页面](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghva5bx7bvj31d10p6thq.jpg)

**歌曲播放功能**：
榜单中歌曲的点击播放；
歌曲控制（暂停、播放、上一首、下一首、进度改变）；
播放循序切换：顺序播放、随机播放、单曲循环；
歌词展示滚动

![歌曲播放](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghv9pc3ki6j30ws0ahti8.jpg)


![排行榜页面](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghv9qjg0m4j31d10p4ai3.jpg)



![新碟上架页面](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghv9uryexgj31d10p4aue.jpg)



### 1.2. 项目相关技术概要

* CSS采用普通CSS和styled-component结合
* 项目统一使用函数式组件和Hooks，并且组件全部使用memo包裹，减少不必要的渲染
* 组件内部状态，使用useState、useReducer；业务数据放在redux管理；
* redux结合ImmutableJS，异步请求代码使用redux-thunk，redux采用redux hooks方式编写
* 网络请求采用二次封装的axios
* 使用AntDesign编写部分组件

### 1.3. 项目运行

clone项目：

```
git clone https://github.com/Hendry5479/react-netease-music.git
```

安装项目依赖：

```shell
yarn install
```

项目运行：

```shell
yarn start
```



