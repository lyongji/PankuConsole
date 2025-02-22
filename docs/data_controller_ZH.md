# 数据控制器

![](./assets/data_controller.png)

您可以直接从可用对象生成数据控制器窗口。可以在数据控制器窗口中修改变量的值，同时数据控制器窗口会实时更新变量的值，这是一个双向数据绑定。

您只需在[开发者控制台](./developer_console.md)中输入对象表达式即可创建一个数据控制器。例如，如果您在开发者控制台中输入current并且场景根脚本包含导出变量，则会根据导出变量自动创建一个数据控制器。

> 值得注意的是，[通用设置](./general_settings.md)窗口（通过general_settings.open()创建）也是由数据控制器生成的。

## 支持的类型

当前支持的导出变量类型如下所示。

`gdscript

#以下划线开头的导出变量将被忽略。
@export var _ignored := 0

#0. 分组按钮
@export_group( Group 1)

#1. 滚动字幕单行注释。名称需要以xport_comment_开头。
@export var export_comment_1 = 这是一个注释

#2. 按钮。名称格式应为xport_button_xxx，其中xxx是点击按钮时调用的同一文件中的函数名称。
@export var export_button_xxx = 点击我

#3. 布尔变量。
@export var bool_val:bool = false

#4. 颜色变量。
@export var color_val:Color = Color.WHITE

#5. 字符串变量。
@export var string_val:String = "

#6. 简单整数变量。
@export var int_val:int = 0

#7. 简单浮点数变量。
@export var float_val:float = 0

#8. 带范围的数值（整数或浮点数）变量。
@export_range(0.0, 1.0, 0.01) var ranged_number := 0.0

#9. Vector2变量。
@export var vec2_val:Vector2 = Vector2.ZERO

#10. 枚举整数值
@export_enum(选项1, 选项2, 选项3) var enum_val := 0

#11. 不支持的变量将显示为只读字符串。
@export var node_val:Node

#12. 您可以使用setget函数控制访问行为。
@export var dummy_val:int:
    set(val): pass
    get: return 0

#按钮回调函数
func xxx():
    print(xxx被调用)

`

## 相关文件

panku_console/modules/data_controller/*
