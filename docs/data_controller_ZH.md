# ���ݿ�����

![](./assets/data_controller.png)

������ֱ�Ӵӿ��ö����������ݿ��������ڡ����������ݿ������������޸ı�����ֵ��ͬʱ���ݿ��������ڻ�ʵʱ���±�����ֵ������һ��˫�����ݰ󶨡�

��ֻ����[�����߿���̨](./developer_console.md)�����������ʽ���ɴ���һ�����ݿ����������磬������ڿ����߿���̨������current���ҳ������ű��������������������ݵ��������Զ�����һ�����ݿ�������

> ֵ��ע����ǣ�[ͨ������](./general_settings.md)���ڣ�ͨ��general_settings.open()������Ҳ�������ݿ��������ɵġ�

## ֧�ֵ�����

��ǰ֧�ֵĵ�����������������ʾ��

`gdscript

#���»��߿�ͷ�ĵ��������������ԡ�
@export var _ignored := 0

#0. ���鰴ť
@export_group( Group 1)

#1. ������Ļ����ע�͡�������Ҫ��xport_comment_��ͷ��
@export var export_comment_1 = ����һ��ע��

#2. ��ť�����Ƹ�ʽӦΪxport_button_xxx������xxx�ǵ����ťʱ���õ�ͬһ�ļ��еĺ������ơ�
@export var export_button_xxx = �����

#3. ����������
@export var bool_val:bool = false

#4. ��ɫ������
@export var color_val:Color = Color.WHITE

#5. �ַ���������
@export var string_val:String = "

#6. ������������
@export var int_val:int = 0

#7. �򵥸�����������
@export var float_val:float = 0

#8. ����Χ����ֵ�������򸡵�����������
@export_range(0.0, 1.0, 0.01) var ranged_number := 0.0

#9. Vector2������
@export var vec2_val:Vector2 = Vector2.ZERO

#10. ö������ֵ
@export_enum(ѡ��1, ѡ��2, ѡ��3) var enum_val := 0

#11. ��֧�ֵı�������ʾΪֻ���ַ�����
@export var node_val:Node

#12. ������ʹ��setget�������Ʒ�����Ϊ��
@export var dummy_val:int:
    set(val): pass
    get: return 0

#��ť�ص�����
func xxx():
    print(xxx������)

`

## ����ļ�

panku_console/modules/data_controller/*
