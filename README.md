# Godot-notes
Godot的笔记整理，基于版本4.2

## 说明

在godot中，有时候会遇到一些代码不生效的情况，此时可尝试重启项目

## 文档说明

* `Callable bind(...) vararg const`
  * 在这个方法声明中`...`和`vararg`同时出现，表示可选参数
  * `const`表示返回值为一个常量

* `Variant`表示任意类型的数据

* `void _draw() virtual`
  * 在这个方法声明中
  * `virtual`表示是可以被重写的方法
  * 一般以`_`开头的内置方法都可以被重写
