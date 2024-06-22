# `Sprite2D`

普通的精灵节点

## 属性

* `texture`
  * `Texture2D texture`
  * 精灵的纹理
* `hframes`
  * `int hframes [default: 1]`
  * 精灵集的列数
* `vframes`
  * `int vframes [default: 1]`
  * 精灵集的行数
* `frame`
  * 表示展示精灵集中的第几个
  * 动态切换这个值，可以通过`Sprite2D`实现动画效果
  * 原理类似于电影的胶卷