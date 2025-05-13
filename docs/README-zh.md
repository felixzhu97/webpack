<div align="center">
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200" src="https://webpack.js.org/assets/icon-square-big.svg">
  </a>
  <br>
  <br>

[![npm][npm]][npm-url]

[![node][node]][node-url]
[![builds1][builds1]][builds1-url]
[![builds2][builds2]][builds2-url]
[![dependency-review][dependency-review]][dependency-review-url]
[![coverage][cover]][cover-url]
[![PR's welcome][prs]][prs-url]

<h1>webpack</h1>
<p>
  webpack 是一个模块打包工具。它的主要目的是将 JavaScript 文件打包用于浏览器使用，但它也能够转换、打包或包装几乎任何资源或资产。
</p>
</div>

## 目录

- [安装](#安装)
- [介绍](#介绍)
- [核心概念](#核心概念)
- [贡献](#贡献)
- [支持](#支持)
- [赞助](#赞助)

<h2>安装</h2>

使用 npm 安装:

```bash
npm install --save-dev webpack
```

使用 yarn 安装:

```bash
yarn add webpack --dev
```

<h2>介绍</h2>

webpack 是一个模块打包工具。主要目的是打包 JavaScript 文件供浏览器使用，但它也能够转换、打包几乎任何类型的资源。

**核心功能**

- 支持 ES Modules、CommonJS 和 AMD 模块
- 可以创建单个包或多个异步加载的块（减少初始加载时间）
- 依赖关系在编译时解析，减少运行时大小
- 加载器可以在编译时预处理文件
- 高度模块化的插件系统

### 快速开始

查看 webpack 的 [快速开始](https://webpack.js.org/guides/getting-started) 指南。

<h2>核心概念</h2>

### [插件](https://webpack.js.org/plugins/)

webpack 拥有丰富的插件接口，大多数功能都使用这个插件接口实现。

### [加载器](https://webpack.js.org/loaders/)

webpack 支持使用加载器预处理文件，允许打包任何静态资源。

### 代码分割

webpack 允许将代码库拆分为多个块，这些块在运行时异步加载，减少初始加载时间。

### 性能优化

webpack 可以进行多种优化来减少 JavaScript 输出大小。

<h2>贡献</h2>

我们欢迎任何形式的贡献，包括：

- 文档更新和改进
- 问题修复
- 新功能开发
- 测试用例添加

查看我们的 [贡献指南](https://github.com/webpack/webpack/blob/main/CONTRIBUTING.md) 了解更多。

<h2>支持</h2>

如果您遇到问题或有功能建议，请在 GitHub 上创建 issue。

<h2>赞助</h2>

webpack 是一个开源项目，欢迎赞助支持开发。

[npm]: https://img.shields.io/npm/v/webpack.svg
[npm-url]: https://npmjs.com/package/webpack
[node]: https://img.shields.io/node/v/webpack.svg
[node-url]: https://nodejs.org
[prs]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg
[prs-url]: https://webpack.js.org/contribute/
[builds1]: https://github.com/webpack/webpack/actions/workflows/test.yml/badge.svg
[builds1-url]: https://github.com/webpack/webpack/actions/workflows/test.yml
[builds2]: https://dev.azure.com/webpack/webpack/_apis/build/status%2Fwebpack.webpack?branchName=main
[builds2-url]: https://dev.azure.com/webpack/webpack/_build/latest?definitionId=3&branchName=main
[dependency-review-url]: https://github.com/webpack/webpack/actions/workflows/dependency-review.yml
[dependency-review]: https://github.com/webpack/webpack/actions/workflows/dependency-review.yml/badge.svg
[cover]: https://codecov.io/gh/webpack/webpack/graph/badge.svg?token=mDP3mQJNnn
[cover-url]: https://codecov.io/gh/webpack/webpack
