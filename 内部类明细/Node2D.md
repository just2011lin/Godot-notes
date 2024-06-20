# `Node2D`

所有2D相关节点的基类，包含位置、旋转、缩放和z_index信息

## 属性

* `global_position`
  * `Vector2 global_position`
  * 全局位置
  * 个人感觉此方式只是为了方便的设置`position`
  * 本质上是将`global_position`转为`position`后设置`position`

* `position`
  * `Vector2 position[0, 0]`
  * 相对于父节点的位置

* `to_global`
  * `Vector2 to_global(local_potin: Vector2) const`
  * 将本地相对于父节点的坐标，转变为在全局下的坐标

* `to_local`
  * `Vector2 to_local(global_point: Vector2) const`
  * 将全局下的坐标转变为基于父节点的坐标
