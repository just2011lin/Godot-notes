# Gdscript语法

* in操作符

```
# 检查对象中是否存在属性、方法或信号名称
"name" in node
```

* extend继承

```
# 表明继承自某个节点
extend Sprite2D
```

* _方法

```
# 内部类中_开头的方法，可以是可以重写的方法
```

* _not取反

```
# 使用not对值取反
not true
```

* signal定义信号
```
signal health_depleted
```

* await等待信号
```
# 等待一个定时器触发
await timer.timeout
```

* $获取
```
# 相当于使用get_node
$Child 等同于 get_node("Child")
$"../" 等同于 get_node("../")，也等同于 get_parent()
```

* 指定类型
```
var floor: PackedScene
```

* `setter`与`getter`
```
var m_name:
    set(value):
        m_name = value
    get:
        return "Lucy"
```

* @onready
```
# 在方法外不能使用$获取
# @onready注解使赋值相当于在`_ready`f中进行
@onready var sub_node = $SubNode
```
