# Timer

定时器实现

## 属性

* `auto_start`
  * `bool autostart [default: false]`
  * 是否自动启动
* `one_shot`
  * `bool one_shot [default: false]`
  * 是否只触发一次
  * 值为`false`时，会重复触发
* `wait_time`
  * `float wait_time [default: 1.0]`
  * 等待时间，单位：秒，默认值为1秒

## 信号

* `time_out`
  * 当`wait_time`时间到了后触发

## 方法

* `start`
  * `void start(time_sec: float = -1)`
  * 启动定时器
  * 可以通过参数`time_sec`设定`wait_time`
* `stop`
  * `void stop()`
  * 停止定时器