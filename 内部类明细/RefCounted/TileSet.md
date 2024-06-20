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