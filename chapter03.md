# 布局

## 常用布局方法

- table 表格布局
- float 浮动 + margin
- inline-block 布局
- flexbox 布局

## 盒模型

![](https://i.loli.net/2019/04/11/5caeedc7a7543.png)

- content 内容显示区域 设置宽高
- padding 内容区到边框
- border 边框 本身也是占据空间的
- margin 离别的元素的距离

## display/position

- display 确定元素的显示类型
  - block/inline/inline-block
- position 确认元素的位置
  - static/relative/absolute/fixed (fixed 固定位置。默认 static 静态位置)
  - 通过设置 z-index 体现优先级 (relative/absolute/fixed 可以设置 注意 static 并不能)

## flexbox

- 弹性盒子
- 盒子本来就是并列的
- 指定宽度即可

## float 浮动布局

- 元素“浮动”
- 脱离文档流
- 但不脱离文本流
- 常用于图文混排
- 对自身的影响：
  - 形成“块”（BFC）
  - 位置尽量靠上
  - 位置尽量靠左（右）
- 对兄弟元素的影响：
  - 上面贴非 float 元素
  - 旁边贴 float 元素
  - 不影响其他块级元素位置
  - 影响其他块级元素内部文本
- 对父级元素的影响
  - 从布局上“消失”
  - 高度塌陷