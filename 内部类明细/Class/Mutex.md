# Mutex

在多线程中实现同步机制的信号

* 基本使用方式

  * 在两个线程中，使用同一个`mutex`

  * 当`mutext`调用`lock`后且未完全`unlock`时
  * 其它地方再调用`lock`时不会继续执行下面的代码
  * 直到`mutext`调用`unlock`解除一个`lock`时
  * 原先被`lock`处才会继续执行

## 方法

* `lock`
  * `void lock()`
* `unlock`
  * `void unlock()`

