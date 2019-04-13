# CSS 工程化

- 组织
- 优化
- 构建
- 维护

## PostCSS

![](https://i.loli.net/2019/04/13/5cb1d68229225.png)

- postcss 本身只有解析能力
- 各种神奇的特性全靠插件

- postcss-import 模块合并
- autoprefixier 自动加前缀
- cssnano 压缩代码
- cssnext 使用 css 新特性
- precss 变量、mixin、循环等

## webpack

- JS 是整个应用的核心入口
- 一切资源均由 JS 管理依赖
- 一切资源均由 webpack 打包

### webpack 和 CSS

- css-loader 将 CSS 变成 JS
- style-loader 将  JS 样式插入 html 中的 head
- ExtractTextPlugin 将 CSS 从 JS 中提取出来
- css modules 解决 CSS 命名冲突的问题
- less-loader sass-loader 各类预处理器
- postcss-loader PostCSS 处理

## CSS 面试真题

### 如何解决 CSS 模块化问题

- less sass 等 css 预处理器
- postcss 插件 (postcss-import/precss 等)
- webpack 处理 css (css-loader + style-loader)

### PostCSS 可以做什么

- 取决于插件可以做什么
- autoprefixer cssnext precss 等 兼容性处理
- import 模块合并
- css 语法检查 兼容性检查
- 压缩文件

### CSS modules 是做什么的，如何使用

- 解决类名冲突的问题
- 使用 PostCSS 或者 webpack 等构建工具进行编译
- 在 HTML 模版中使用编译过程产生的类名

### 为什么使用 JS 来引用、加载 CSS

- JS 作为入口，管理资源有天然优势
- 将组件的结构、样式、行为封装到一起，增加内聚
- 可以做更多处理（webpack）