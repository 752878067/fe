# CSS 动画

`CSS3` CSS 动画可能是 CSS 中最有趣的部分。

## transition
[transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition) 属性用于设置元素两种状态间的过渡动画，是以下四个属性的缩写。
* [transition-property](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-property) 属性用于设置动画属性。
* [transition-duration](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-duration) 属性用于设置动画时长。
* [transition-timing-function](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function) 属性用于设置动画时间函数。
* [transition-delay](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-delay) 属性用于设置动画延时。

```css
.😎 {
  /* (所有)属性 | 时长 | 函数 | 延时 */
  transition: all 0.5s ease-out .2s;
}
```

**注意** 只有一部分 CSS 属性是可以 “动” 的，详见 MDN [CSS Animated Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties)。

## transform
[transform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform) 用于
* `none`
* `translate()` 🌰 `translate(20px, 30%);`
* `translateX()`
* `translateY()`
* `translateZ()`
* `translate3d()`
* `skew()`
* `skewX()`
* `skewY()`
* `scale()`
* `scaleX()`
* `scaleY()`
* `scaleZ()`
* `scale3d()`
* `rotate()`
* `rotateX()`
* `rotateY()`
* `rotateZ()`
* `rotate3d()`
* `matrix()`
* `matrix3d()`

[transform-style](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-style) 用于设置元素的子元素(s)是处于 3D 空间还是平面空间。
* `flat` 平面空间
* `preserve-3d` 3D 空间

[transform-origin](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-origin)

## perspective
[perspective](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective)

## backface-visibility
[backface-visibility](https://developer.mozilla.org/en-US/docs/Web/CSS/backface-visibility)

## @keyframes
[@keyframes](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes) 用于自定义动画帧。

```css
@keyframes tooltip-appear {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}
```

## animation
[animation](https://developer.mozilla.org/en-US/docs/Web/CSS/animation) 属性用于设置应用在元素上的动画，是以下属性的缩写。
* [animation-name](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-name)
* [animation-duration](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-duration)
* [animation-timing-function](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-timing-function)
* [animation-delay](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-delay)
* [animation-iteration-count](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-iteration-count)
* [animation-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-direction)
* [animation-fill-mode](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-fill-mode)
* [animation-play-state](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-play-state)

## 开源项目
* [Animate.css](https://daneden.github.io/animate.css/)

## 参考链接
* https://davidwalsh.name/css-flip
* https://css-tricks.com/almanac/properties/a/animation/
* https://developer.mozilla.org/en-US/docs/Web/CSS/transition
* https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties
* https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions

