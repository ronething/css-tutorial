# 预处理器

- 基于 CSS 的另一种语言
- 通过工具编译成 CSS
- 添加了很多 CSS 不具备的特性
- 能提升 CSS 文件的组织方式

- 嵌套 反应层级和约束
- 变量和计算 减少重复代码
- Extend 和 Mixin 代码片段
- 循环 适用于复杂有规律的样式
- import CSS 文件模块化

## less

### 编译

- `./node_modules/.bin/lessc demo01.less `

### 变量

- `@var: xxx`

### mixin

- css 层面代码复用

  ```css
  .block(@fontSize) {
    font-size: @fontSize;
  }
  ```

### extend

- 和 `mixin` 相比 不是复制 而是提取。重复的内容变少了。
- `&:extend(.block)`

### loop

- 不支持 `for` 循环
- `mixin` 方式

### import

- `@import 'xxx'`

## scss

### 编译

- `./node_modules/.bin/node-sass demo01.scss`

### 变量

- `$var: xxx`

### mixin

- 声明 `@mixin name{}`
- 调用 `@include name()`

### extend

-  `@extend .block;`

### loop

- 支持 `for` 循环

### import

- 同 `less`

## 预处理器框架

- sass - compass
- less- lesshat/EST
- 提供现成的 mixin
- 类似 JS 类库 封装常见功能

## CSS 面试真题

### 常见的 CSS 预处理器

- Less(Node.js)
- Sass(Ruby 有 Node 版本)

### 预处理器的作用

- 帮助更好地组织 CSS 代码
- 提高代码复用率
- 提升可维护性

### 预处理器的能力

- 见上文

### 预处理器的优缺点

- 优点：提高代码复用率和可维护性
- 缺点：需要引入编译过程 有学习成本