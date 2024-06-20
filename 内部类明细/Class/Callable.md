# Callable

内置类型，表示方法或单独的函数

## 构造

* `Callable(object: Object, method: StringName)`
  * `Dictionary`类型的值，不能作为第一个参数

## 方法

* ` bind`
  * `Callable bind(...) vararg const`
  * 方法绑定多个参数，然后返回一个新的方法
  * 需注意参数传入的顺序

* `call`
  * `Variant call(...) vararg const`
  * 调用方法，并可以传入参数