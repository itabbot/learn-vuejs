# 最简单的 Vue 单页应用<!-- omit in toc -->

- [1. 搭建](#1-搭建)
  - [1.1. 准备工作](#11-准备工作)
  - [1.2. 执行 Vue 官方的项目脚手架工具](#12-执行-vue-官方的项目脚手架工具)
  - [1.3. 安装依赖](#13-安装依赖)
  - [1.4. 编译和热重载（用于开发）](#14-编译和热重载用于开发)
  - [1.5. 编译和压缩（用于生产）](#15-编译和压缩用于生产)
- [2. 理解](#2-理解)

## 1. 搭建

### 1.1. 准备工作

安装 16.0 或更高版本的 [Node.js](https://nodejs.org)。

### 1.2. 执行 Vue 官方的项目脚手架工具

```sh
> npm init vue@latest

Need to install the following packages:
  create-vue@latest
Ok to proceed? (y)

Vue.js - The Progressive JavaScript Framework

√ Project name: ... simplest-SPA
√ Package name: ... simplest-spa
√ Add TypeScript? ... No
√ Add JSX Support? ... No
√ Add Vue Router for Single Page Application development? ... No
√ Add Pinia for state management? ... No
√ Add Vitest for Unit Testing? ... No
√ Add an End-to-End Testing Solution? » No
√ Add ESLint for code quality? ... No

Scaffolding project in ./simplest-SPA...

Done. Now run:

  cd simplest-SPA
  npm install
  npm run dev
```

### 1.3. 安装依赖

```sh
> npm install
```

### 1.4. 编译和热重载（用于开发）

```sh
> npm run dev

VITE v4.2.1  ready in 362 ms

  ➜  Local:   http://127.0.0.1:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help
```

### 1.5. 编译和压缩（用于生产）

```sh
> npm run build

vite v4.2.1 building for production...
✓ 23 modules transformed.
dist/assets/logo-277e0e97.svg    0.28 kB
dist/index.html                  0.42 kB
dist/assets/index-1da8cd0c.css   3.68 kB │ gzip:  1.20 kB
dist/assets/index-a911f458.js   62.95 kB │ gzip: 24.96 kB
✓ built in 873ms
```

## 2. 理解

使用 Vue 官方脚手架工具搭建的该项目：

- 使用了 [Vite](https://cn.vitejs.dev) 构建工具。
- 以 `index.html` 作为入口文件，Vite 解析其 `<script type="module" src="...">` 标签指向 JavaScript 源码 `./src/main.js`。
- 在 `./src/main.js` 中引入样式表 `./src/assets/main.css`。
- 在 `./src/main.js` 中以 `./src/App.vue` 作为根组件创建 Vue 应用实例，并挂载在 `#app` 元素之上。
