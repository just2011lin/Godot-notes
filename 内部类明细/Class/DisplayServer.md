# DisplayServer

单例，跟窗口有关的信息管理，可以理解为`OS`中分离出来的一些方法集合

## 方法

* `window_get_size`
  * `Vector2i window_get_size(window_id: int = 0) const`
  * 获取窗口的尺寸