# 框架中的 CSS

## Angular

### ShadowDOM

- 逻辑上一个 DOM(例如 video 标签)
- 结构上存在子集结构

### Scoped CSS

- 限定了范围的 CSS
- 无法影响外部元素
- 外部样式一般不影响内部
- 可以通过 /deep/ 或 >>> 穿透

### 模拟 Scoped CSS

- 随机选择器(Angular 不支持 vue 支持)
  - css modules
- 随机属性
  ```css
  <div abcdefg>
  div[abcdefg]{}
  ```

## Vue

- 默认采用随机属性
- css modules `<style module>` `$style.xxx`