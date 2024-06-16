# Object

## 描述

* 所有类的基类
* 提供了`_init`方法
  * 当子类调用`new`时，实际调用的是`_init`
* 提供了`free`方法，用于删除自身
* 关于内存管理
  * 只有`RefCounted`类会使用引用计数的方式回收垃圾
  * free一个`Node`节点时，会同步删除其子节点
* 对象可以添加脚本
* `set_script`方法，可以在运行时更改对象的脚本
* 属性、方法和信号也可以在运行时中更改
* `notifycation`方法，会触发所有节点的`_notifycation`方法
  * 实际测试下来，发现第二个参数`reversed`未生效
* 可以使用`set_meta`来保存对属性的描述信息，不建议过渡使用
* 检测对象是否存在，应该使用全局的`is_instance_valid`
  * 实际测试下来，此方法不能检测数字或字符串是否存在
  * 可能是检测值是否为Object实例

## 信号

* property_list_changed()
  * 当调用`notify_property_list_changed`时触发
  * 在编辑器链接该信号，可能会导致检查器中不能显示`@export`变量
* script_changed()
  * 当节点的脚本发生改变时触发

## _方法

* `_get_property_list`此方法可以自定义属性在检查器面板中的展示
  * 经过尝试，`_get_property_list`方法描述中的例子需要重启项目后才能生效
* `_init`方法，相当于对象的构造函数，可以设定和接收参数
* `_property_can_revert`和`_property_get_revert`可以定义检查器面板中属性的重置行为
* `_set`配合`_get`和`_get_property_list`可以自定义属性的赋值和获取
* `_to_string`方法定义对象转为字符串后的结果
* 通知属性列表变化后，先调用`_get_property_list`获取属性列表，再经过`_validate_property`方法对属性列表做出更改

## 方法

* `add_user_signal`方法，用于动态添加一个信号
* `call`方法，可用于动态控制需要调用的方法
* `call_deferred`方法，设定在空闲后调用一个方法
  * 与`call`返回调用函数的返回值相比，该方法只返回`null`
* `callv`方法，与`call`相比，传入参数的方式不一样
* 

