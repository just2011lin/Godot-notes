# Thread

* `Thread.new()`，创建线程

## 方法

* `get_id`方法
  * `String get_id() const`
  * 获取线程id
* `is_alive`方法
  * `bool is_alive() const`
  * 是否仍在执行任务

* `start`方法
  * `Error start(callable: Callable, priority: Priority = 1)`
  * 使用`Callable.bing()`方式传递额外参数
* `wait_to_finish()`
  * `Variant wait_to_finish()`
  * 等待线程完成，并获取执行结果
  * 也需在释放包含线程的实例前使用
  * 使用`wait_to_finish`后会阻碍后续代码的执行