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
- **清除浮动**
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

## inline-block

- 像文本一样排 block 元素
- 没有清除浮动等问题
- 需要处理间隙（font-sizes）

## 响应式设计和布局

- 在不同设备上正常使用
- 一般主要处理屏幕大小问题
- 主要方法：
  - 隐藏 + 折行 + 自适应空间
  - rem/viewport/media query
  
    media max-width 大的写在前面 反过来的话 小屏幕的样式会被覆盖
    ```css
     @media (max-width: 375px) {
            html {
                font-size: 24px;
            }
        }

        @media (max-width: 320px) {
            html {
                font-size: 20px;
            }
        }
    ```

## CSS 面试真题

### 实现两栏（三栏）布局的方法

- 表格布局
- float + margin 布局
- inline-block 布局
- flexbox 布局

### position:absolute/fixed 有什么区别

- 前者相对最近的 absolute/relative
- 后者相对屏幕（viewport）

### display:inline-block 的间隙

- 原因：空白字符造成字符间距
- 解决：消灭字符(删除空白或者直接注释)或者消灭字距(font-size)

### 为什么需要清除浮动 如何清除浮动

- 防止高度塌陷，不影响其他元素
- 让盒子负责自己的布局
- overflow:hidden(auto)
- ::after{clear:both}

### 如何适配移动端页面

- viewport
- rem/viewport/media query
- 设计上：隐藏 折行 自适应