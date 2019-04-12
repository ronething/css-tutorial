# CSS 动画

## 动画的原理

- 视觉暂留作用
- 画面逐渐变化

## 动画类型

### transition 补间动画

- timing

  ![](https://raw.githubusercontent.com/ronething/Image-Hosting/master/img/20190413000654.png)

  - easy-in-out

  ![](https://raw.githubusercontent.com/ronething/Image-Hosting/master/img/20190413001623.png)

  - linear

  ![](https://raw.githubusercontent.com/ronething/Image-Hosting/master/img/20190413001725.png)

### keyframe 关键帧动画

- 与元素状态的变化无关
- 定义更加灵活

### 逐帧动画

- 没有补间
- 只有关键帧
- 适用于无法补间计算的动画
- 使用 steps(1) 使关键帧之间没有补间

## 面试真题

### CSS 动画的实现方式有几种

- transition
- keyframes(animation)

### 过度动画和关键帧动画的区别

- 过度动画需要有状态变化
- 关键帧动画不需要有状态变化 
- 关键帧动画能控制更精细

### 如何实现逐帧动画

- 使用关键帧动画
- 去掉补间（steps）

### CSS 动画性能

- 性能不坏
- 部分情况下优于 JS
- 但 JS 可以做的更好
- 部分高危属性 box-shadow 等 性能较差 慎用