# Webpack 核心原理

## 1. 模块化系统

Webpack 的核心是一个模块化系统，它支持多种模块规范：

- ES Modules (import/export)
- CommonJS (require/module.exports)
- AMD (define/require)

Webpack 将所有模块视为依赖关系图中的节点，通过静态分析建立完整的依赖关系。

## 2. 编译过程

Webpack 的编译过程分为几个关键阶段：

1. **解析(Resolution)**:

   - 从入口文件开始，解析模块路径
   - 使用解析器(resolver)定位模块的绝对路径

2. **加载(Loading)**:

   - 通过对应的加载器(loader)处理模块内容
   - 支持转换各种资源类型(JS, CSS, 图片等)

3. **构建(Build)**:

   - 创建模块依赖图(Dependency Graph)
   - 执行代码转换和优化

4. **分块(Chunking)**:

   - 根据配置和动态导入拆分代码块
   - 实现代码分割(Code Splitting)

5. **输出(Output)**:
   - 生成最终打包文件
   - 写入到配置的输出目录

## 3. 关键组件

### 3.1 入口(Entry)

定义应用程序的起点，Webpack 从这里开始构建依赖图。

### 3.2 输出(Output)

配置打包文件的输出位置和命名规则。

### 3.3 加载器(Loaders)

用于转换非 JavaScript 模块，将其转换为 Webpack 能够处理的模块。

### 3.4 插件(Plugins)

扩展 Webpack 功能，可以介入到编译过程的各个阶段。

### 3.5 模式(Mode)

通过设置 development 或 production 模式，启用相应的优化。

## 4. 依赖图(Dependency Graph)

Webpack 的核心数据结构是依赖图，它：

- 以入口点为起点
- 递归解析所有依赖关系
- 将整个应用表示为一个依赖关系图
- 最终生成优化的打包文件

## 5. 热更新(Hot Module Replacement)

Webpack 的热更新机制允许：

- 在不刷新页面的情况下更新模块
- 保持应用状态
- 提高开发效率

## 6. 代码分割(Code Splitting)

Webpack 提供多种代码分割方式：

- 入口点分割
- 动态导入(dynamic import)
- 防止重复(SplitChunksPlugin)

## 7. 优化策略

Webpack 包含多种优化策略：

- Tree Shaking (移除未使用代码)
- Scope Hoisting (作用域提升)
- 代码压缩
- 缓存优化

## 8. 运行时(Runtime)

Webpack 生成的运行时包含：

- 模块加载逻辑
- 模块缓存系统
- 热更新支持
- 代码分割支持

通过理解这些核心原理，可以更好地配置和使用 Webpack，充分发挥其模块化打包的能力。
