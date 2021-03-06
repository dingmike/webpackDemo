# SoEasy-Webpack4.0-Templete

v2.0版本之后，本项目暂停更新维护，但不影响使用。现侧重基于Vue模板开发，如果您是Vue.js技术栈，请转移至 SoEasy-Vue-Webpack-Templete 项目: https://github.com/ycmbcd/SoEasy-Vue-Webpack-Templete

# 使用

> npm

```bash
# 初始化
npm install

# 开发模式
npm run dev

# 构建
npm run build
```

> cnpm

```bash
# 初始化
cnpm install

# 开发模式
cnpm run dev

# 构建
cnpm run build
```

> yarn

```bash
# 初始化
yarn

# 开发模式
yarn run dev

# 构建
yarn run build
```

# 预览

[Demo](https://ycmbcd.github.io/SoEasy-Webpack4.0-Templete/dist/)

# 说明

一款开箱即用的基于 `Webpack 4.0` 搭建的 `WebApp` 模板。

> 目录说明

```bash
SoEasy-Webpack4.0-Templete
├─ .babelrc                     #babel配置文件
├─ dist                         #构建目录
│  ├─ favicon.ico               #构建后的图标文件
│  ├─ index.html                #构建后的主页
│  └─ static                    #构建后的静态目录
│     ├─ css                    #构建后的样式目录
│     │  └─ main_021153.css     #构建后的测试样式文件
│     ├─ images                 #构建后的图片目录
│     │  └─ panda_eb8547.png    #构建后的测试图片文件
│     └─ js                     #构建后的JS目录
│        ├─ main_056c80.js      #构建后的测试JS文件
│        └─ main_056c80.js.map  #构建后的测试JS地图文件
├─ favicon.ico                  #图标文件
├─ index.html                   #主页
├─ node_modules                 #包目录
├─ package.json                 #项目文件
├─ src                          #开发源码目录
│  ├─ add.js                    #Demo测试文件
│  └─ stylus                    #Stylus目录
│     └─ custom.styl            #Demo测试styl文件
│  ├─ assets                    #开发资源目录
│  │  └─ images                 #开发图片目录
│  │     ├─ panda.png           #Demo测试图片
│  │     └─ phone.jpg           #Demo测试图片
│  ├─ main.css                  #Demo测试样式
│  └─ main.js                   #入口文件
├─ webpack.common.js            #Webpack基础配置文件
├─ webpack.dev.js               #Webpack开发配置文件
└─ webpack.prod.js              #Webpack生产配置文件
```

# 特色

- 配置文件分离，生产 `production` 模式、开发 `development` 模式，适合大中型应用开发。
- 配置项目清晰明了，适合初学者上手。
- `/src` 文件夹自带 `Demo`，`yarn run dev` 后，会在浏览器打开一个 `Demo` 运行界面判断插件加载器是否正常运行。

# 配置

- webpack.coommon.js 公共配置文件
- webpack.dev.js 开发 `development` 模式配置文件
- webpack.prod.js 生产 `production` 模式配置文件

> 运行脚本配置： package.json

```json
"scripts": {
    "build": "webpack --config webpack.prod.js",
    "dev": "webpack-dev-server --config webpack.dev.js"
},
```

# 功能

- 支持 ES6 编译 ES5。
- Js 文件压缩，sourse-map 分配。
- ~~支持 Sass/Scss 编译。~~（node-sass 加载慢顾改用Stylus。如需Sass请使用 `v2.0` 之前的版本。）
- 支持 Stylus 编译。
- CSS 样式分离、压缩。
- CSS3 前缀自动补全。
- 图片小于 10kb 进行 `base64` 转码。
- 支持字体文件的打包。
- 支持模块自动加载。
- 打包文件哈希值分配，便于部署更新。
- 支持热更新「HMR」，默认端口：8080。
- 默认支持 `favicon.ico` 打包。
- 支持 `.editorconfig` 编辑器格式统一标准。

# 许可
MIT License
