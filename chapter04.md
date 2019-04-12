# 效果属性

## box-shadow 

- 营造层次感（立体感）
- 充当没有宽度的边框
- 特殊效果（投影）

## text-shadow

- 立体感
- 印刷品质感

## border-radius

- 圆角举行
- 圆形
- 半圆/扇形

## background

- 纹理、图案
- 渐变
- 雪碧图动画
- 背景图尺寸适应

  ```css
  background-size: 20px 10px;
  background-size: 100% 100%;
  background-size: cover/contain;
  background-repeat: no-repeat;
  background-position: center center;
  ```

## clip-path

- 对容器进行裁剪
- 常见几何图形
- 自定义路径 svg

## 3D 变换

- 在 3D 空间中进行变换
- 性能一般

## 面试真题

### 如何用一个 div 画 XXX

- box-shadow 无限投影
- ::before
- ::after

### 如何产生不占空间的边框

- box-shadow
- outline

### 盒子宽度包含边框

- box-sizing: border-box

### 如何实现圆形元素（头像）

- border-radius: 50%;

### 如何实现 IOS 图标的圆角

![](https://i.loli.net/2019/04/12/5cb08b93515e7.png)

### 如何实现背景图居中显示/不重复/改变大小

- background-position
- background-repeat
- background-size(cover/contain)

### 如何平移/放大一个元素

- transform:translateX(100px)
- transform:scale(2)

### 如何实现 3D 效果

- perspective: 500px
- transform-style: preserve-3d
  前两步准备 3D 场景
- transform: translate rotate