# `Vector2D`

使用浮点数作为x和y的2D向量

## 属性

* `float x`
* `float y`

## 方法

* `normalized`
  * `Vector2 normalized() const`
  * 等同于`v / v.length()`
  * 返回同方向上长度为1的向量
* `dot`
  * `float dot(with: Vector2) const`
  * 向量的点积
* `cross`
  * `float cross(with: Vector2) const`
  * 向量的叉积
* `angle_to`
  * `float angle_to(to: Vector2) const`
  * 向量的夹角

## 运算符

* `+`号
  * `v1 + v2` 等同于 `Vector2(v1.x + v2.x, v1.y + v2.y)`
* `-`号
  * `v1 - v2`等同于`Vector2(v1.x - v2.x, v1.y - v2.y)`
* `*`号
  * `v1 * number`等同于`Vector2(v1.x * number, v1.y * number)`
  * `v1 * v2`等同于`Vector2(v1.x * v2.x, v1.y * v2.y)`