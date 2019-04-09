## HTML 元素分类

### 按默认样式分

- block 块级 独占一行 有形状有尺寸 div p article
- inline 行内 span em strong
- inline-block 对外 inline 对内 block | select input

### 按内容分

![](https://raw.githubusercontent.com/ronething/Image-Hosting/master/img/20190407143443.png)

## HTML 元素嵌套关系

- 块级元素可以包含行内元素
- 块级元素不一定能包含块级元素
- 行内元素**一般**不能包含块级元素

> 为什么 a>div 是合法的？

html5 中 a 为 Transparent （透明）元素 Some elements are described as transparent; they have "transparent" in the description of their content model. 

## HTML 面试真题

- doctype 的意义是什么

    - 让浏览器以标准模式渲染
    - 让浏览器知道元素的合法性

- HTML XHTML HTML5 的关系

    - HTML 属于 SGML
    - XHTML 属于 XML，是 HTML 进行 XML 严格化的结果
    - HTML5 不属于 SGML 或 XML，比 XHTML 宽松

- HTML5 有什么变化

    - 新的语义化元素
    - 表单增强
    - 新的 API（离线、音视频、图形、实时通信、本地存储、设备能力）
    - 分类和嵌套变更

- em 和 i 有什么区别

    - em 是语义化的标签，表强调
    - i 是纯样式的标签，表斜体
    - HTML5 中不推荐使用 i，一般用作图标

- 语义化的意义是什么

    - 开发者容易理解
    - 机器容易理解结构（搜索、读屏、软件）
    - 有助于 SEO
    - semantic microdata 进一步语义化

- 哪些元素可以自闭合
    
    - 表单元素 input
    - 图片 img
    - br hr
    - meta link

- HTML 和 DOM 的关系

    - HTML 是“死”的
    - DOM 由 HTML **解析**而来，是“活”的
    - JS 可以维护 DOM

- property 和 attribute 的区别

    - attribute 是“死”的
    - property 是“活”的 

    ⚠️ attr 和 property 的值不会互相影响

- form 的作用有哪些

    - 直接提交表单
    - 使用 submit/reset 按钮
    - 便于浏览器保存表单
    - 第三方库可以整体提取值
    - 第三方库可以进行表单验证
    