# `AStar2D`

A*算法的实现，适用于2D网格类游戏

## 方法

* `add_point`
  * `void add_point(id: int, position: Vector2, weight_scale: float = 1.0)`
  * 添加一个点
* `connect_points`
  * `void connect_points(id: int, to_id: int, bidirectional: bool = true)`
  * 在两个点之间创建一个线段
* `get_point_ids`
  * `PackedInt64Array get_point_ids()`
  * 返回所有点的id组成的数组
* `get_point_position`
  * `Vector2 get_point_position(id: int) const`
  * 通过id获取点的位置
* `get_point_path`
  * `PackedVector2Array get_point_path(from_id: int, to_id: int)`
  * 获取从from到to的路径

* `has_point`
  * `bool has_point(id: int) const`
  * 通过id判断是否有一个点
* `remove_point`
  * `void remove_point(id: int)`
  * 通过id移除一个点