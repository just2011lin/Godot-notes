# `TileSetAtlasSource`

导出2D图集为一系列瓦片，用作为`TileSet`的资源

## 属性

* `texture`
  * `Texture2D texture`
  * 图片
* `texture_region_size`
  * `Vector2i texture_region_size [default: Vector2i(16, 16)]`
  * 每个瓦片的大小
  * 程序上并不需要比`TileSet`的`tile_size`大

## 方法

* `create_tile`
  * `void create_tile(atlas_coords: Vector2i, size: Vector2i = Vector2i(1, 1))`
  * 创建瓦片，只有调用此方法创建后才会有瓦片
  * 其中的`atlas_coords`是指基于`texture_region_size`的网格坐标，并非像素坐标
  * `size`的默认值为一个瓦片的大小，实际大小要乘以`texture_region_size`