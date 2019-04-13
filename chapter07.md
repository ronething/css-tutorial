# Bootstrap

- 一个 CSS 框架 提供通用基础样式
- 兼容 IE10+
- 使用 flexbox 布局
- 抛弃 Normalize.css
- 提供布局和 reboot 版本

## JS 组件

- 基于 data-* 属性
- 基于 JS API

## 响应式布局

![](https://i.loli.net/2019/04/13/5cb19bd842d62.png)

- class prefix

## 定制化

- 使用 CSS 同名类覆盖
- 修改源码重新构建（3.x 以下使用 less，4 使用 scss）
- 引用 scss 源文件 修改变量

## CSS 面试真题

### Bootstrap 的优缺点

- 优点：CSS 代码结构合理 现成的样式可以直接用
- 缺点：定制较为繁琐 体积大

### Bootstrap 如何实现响应式布局

- 原理：通过 media query 设置不同分辨率的 class
- 使用：为不同分辨率选择不同的网格 class

### 如何基于 Bootstrap 定制样式

- 见上文