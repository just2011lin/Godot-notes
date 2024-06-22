# `Node`

所有场景对象的基类

## 属性

* `owner`
  * 指当前节点所属的场景根节点
  * 场景根节点的`owner`为`null`
  * `add_child`方法添加的节点需手动设置`owner`

## 方法

* `create_tween`
  * `Tween create_tween()`
  * 创建一个`Tween`的实例，并且绑定此节点