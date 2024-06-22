# `Tween`

轻量级的实现一般动画的方式

## 方法

* `set_ease`
  * `Tween set_ease(ease: EaseType)`
  * 设置动画开头和结束时的动画表现形式

* `set_trans`
  * `Tween set_trans(trans: TransitionType)`
  * 设置动画中间状态时的动画表现形式

* `tween_property`
  * `PropertyTweener tween_property(object: Object, property: NodePath, final_val: Variant, duration: float)`
  * 在`duration`时间内，将`object`的`property`值慢慢变为`final_val`
  * 设置多个动画时，会依次执行
* `tween_callback`
  * `CallbackTweener tween_callback(callback: Callable)`
  * 设置动画结束后的回调