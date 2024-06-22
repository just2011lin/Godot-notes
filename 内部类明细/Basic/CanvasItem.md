# `CanvasItem`

抽象类，所有2D类的基类

## _方法

* `_draw`
  * `void _draw() virtual`
  * 此方法内可以调用`draw_*`方法绘制图形
  * 需要注意此方法由引擎自行调用
  * `queue_redraw()`方法调用后，引擎会再次调用`_draw()`方法
  * `draw_*`方法只能在此方法内方可生效

## 方法

* `get_world_2d`
  * `World2D get_world_2d() const`
  * 返回当前项所在的2D世界实例

* `draw_*`
  * 一类方法，可以绘制多种图形
  * 只能在`_draw`方法内调用才可生效
* `queue_redraw`
  * `void queue_redraw()`
  * 该方法调用后，引擎会在合适的时机再次调用`_draw`方法