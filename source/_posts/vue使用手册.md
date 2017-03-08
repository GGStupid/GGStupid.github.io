---
title: vue使用手册
date: 2017-02-28 22:40:45
tags:
	- vue
categories:
	- vue
---
# 安装
<!-- more -->
### 兼容性
Vue不支持IE8以下的浏览器

### 安装
``` bash
npm install vue #最新稳定版
```
重要提示：在开发时请用开发版本，遇到常见错误它会给出友好的警告。
### 独立构建和运行时构建
有两种构建方式，独立构建和运行构建。它们的区别在于前者包含模板编译器而后者不包含。
模板编译用于编译 Vue 模板字符串成纯 JavaScript 渲染函数。如果你想用 template 选项， 你需要编译。
模板编译器的职责是将模板字符串编译为纯 JavaScript 的渲染函数。如果你想要在组件中使用 template 选项，你就需要编译器。
独立构建包含模板编译器并支持 template 选项。 它也依赖于浏览器的接口的存在，所以你不能使用它来为服务器端渲染。
运行时构建不包含模板编译器，因此不支持 template 选项，只能用 render 选项，但即使使用运行时构建，在单文件组件中也依然可以写模板，因为单文件组件的模板会在构建时预编译为 render 函数。运行时构建比独立构建要轻量30%，只有 17.14 Kb min+gzip大小。
默认 NPM 包导出的是 运行时 构建。为了使用独立构建，在 webpack 配置中添加下面的别名：
``` javascript
resolve: {
  alias: {
    'vue$': 'vue/dist/vue.common.js'
  }
}
```
### Vue脚手架工具

``` bash
# 全局安装 vue-cli
$ npm install --global vue-cli
# 创建一个基于 webpack 模板的新项目
$ vue init webpack my-project
# 安装依赖，走你
$ cd my-project
$ npm install
$ npm run dev
```