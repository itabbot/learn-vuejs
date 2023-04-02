# 最简单的 Vue 单页应用<!-- omit in toc -->

- [1. 准备工作](#1-准备工作)
- [2. 执行 Vue 官方的项目脚手架工具](#2-执行-vue-官方的项目脚手架工具)
- [3. 安装依赖](#3-安装依赖)
- [4. 编译和热重载（用于开发）](#4-编译和热重载用于开发)
- [5. 编译和压缩（用于生产）](#5-编译和压缩用于生产)

## 1. 准备工作

安装 16.0 或更高版本的 [Node.js](https://nodejs.org)。

## 2. 执行 Vue 官方的项目脚手架工具

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

## 3. 安装依赖

```sh
> npm install
```

## 4. 编译和热重载（用于开发）

```sh
> npm run dev

VITE v4.2.1  ready in 362 ms

  ➜  Local:   http://127.0.0.1:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help
```

## 5. 编译和压缩（用于生产）

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
