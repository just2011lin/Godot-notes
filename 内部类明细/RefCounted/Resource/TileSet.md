# `TileSet`

`TileMap`的瓦片库

## 属性

* `tile_size`
  * `Vector2i tile_size [default: Vector2i(16, 16)]`
  * 场景中每个格子的大小

## 方法

* `add_source`
  * `int add_source(source: TileSetSource, atlas_source_id_override: int = -1)`
  * 添加一个`TileSetSource`实例
* `add_physics_layer`
  * `void add_physics_layer(to_position: int = -1)`
  * 添加一个物理层
  * 注意：只能按照`0,1,2...`的顺序添加
  * 注意：`to_position`并没有太大意义
* 