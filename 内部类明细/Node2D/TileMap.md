# TileMap

就是TileMap，可用于绘制场景

## 属性

* `tile_set`
  * `TileSet tile_set`
  * 瓦片集

## 方法

* `set_cell`
  * `void set_cell(layer: int, coords: Vector2i, source_id: int = -1, atlas_coords: Vector2i = Vector2i(-1, -1))`
  * 绘制瓦片的方法
  * 特别注意
    * `coords`和`atlas_coords`是坐标
    * 比如`Vector(1, 0)`表示第一行第二个格子
    * 不是像素位置