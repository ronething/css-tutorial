## 选择器

- 用于匹配 HTML 元素
- 分类和权重
- 解析方式和性能 从右往左
- 值得关注的选择器

## 选择器分类

![](https://raw.githubusercontent.com/ronething/Image-Hosting/master/img/20190409152435.png)

## 选择器权重(不进位)

- ID 选择器     +100
- 类 属性 伪类   +10
- 元素 伪元素    +1
- 其他选择器     +0

- !important 优先级最高
- 元素属性 优先级高
- 相同权重 后写的生效

## 非布局样式

- 字体族
    - serif sans-serif monospace
    cursive fantasy
- 多字体 fallback
- 网络字体、自定义字体
- iconfont

## 行高

- 行高的构成

行高由 line-box 组成，line-box 由 inline-box 组成

inline-box 的高度会决定行高

inline 使用 line-height 在 div 中是**垂直居中**的

- 图片缝隙问题

```css
{
    display: block;
}

// 不以为 base line 对齐
{
    vertical-align: bottom;
}
```

## 背景

- 背景颜色
- 渐变色背景
- 多背景叠加
- 背景图片和属性（**雪碧图**）
- base64 和性能优化（一般用于小图标）
- 多分辨率适配

## 边框

- 边框的属性：线型 大小 颜色
- 边框背景图
- 边框衔接（三角形）

## 滚动

- 滚动行为和滚动条

![](https://i.loli.net/2019/04/11/5caec44c8d325.png)

## 文字折行

- overflow-wrap
-  word-break
- white-space

## 装饰性属性及其他

- 字重（粗体）font-weight
- 斜体 font-style:itatic
- 下划线 text-decoration
- 指针 cursor

## CSS Hack

- Hack 即不合法但生效的写法
- 主要用于区分不同浏览器
- 缺点：难理解 难维护 易失效
- 替换方案：特性检测 针对性加 class

### 面试真题

- 雪碧图的作用
  - 减少 HTTP 请求数 提高加载性能
  - 有一些情况下可以减少图片大小

- 自定义字体的使用场景
  - 宣传/品牌/banner 等固定文案
  - 字体图标

- base64 的使用
  - 用于减少 HTTP 请求
  - 适用于小图片
  - base64 的提及约为原图 4/3

- 伪类和伪元素的区别
  - 伪类表示状态
  - 伪元素是真的有元素
  - 前者单冒号，后者双冒号。

- 如何美化 checkbox
  - label[for] 和 id
  - 隐藏原生 input
  - :checked + label