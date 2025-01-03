# Êı¾İ¿ØÖÆÆ÷

![](./assets/data_controller.png)

Äú¿ÉÒÔÖ±½Ó´Ó¿ÉÓÃ¶ÔÏóÉú³ÉÊı¾İ¿ØÖÆÆ÷´°¿Ú¡£¿ÉÒÔÔÚÊı¾İ¿ØÖÆÆ÷´°¿ÚÖĞĞŞ¸Ä±äÁ¿µÄÖµ£¬Í¬Ê±Êı¾İ¿ØÖÆÆ÷´°¿Ú»áÊµÊ±¸üĞÂ±äÁ¿µÄÖµ£¬ÕâÊÇÒ»¸öË«ÏòÊı¾İ°ó¶¨¡£

ÄúÖ»ĞèÔÚ[¿ª·¢Õß¿ØÖÆÌ¨](./developer_console.md)ÖĞÊäÈë¶ÔÏó±í´ïÊ½¼´¿É´´½¨Ò»¸öÊı¾İ¿ØÖÆÆ÷¡£ÀıÈç£¬Èç¹ûÄúÔÚ¿ª·¢Õß¿ØÖÆÌ¨ÖĞÊäÈëcurrent²¢ÇÒ³¡¾°¸ù½Å±¾°üº¬µ¼³ö±äÁ¿£¬Ôò»á¸ù¾İµ¼³ö±äÁ¿×Ô¶¯´´½¨Ò»¸öÊı¾İ¿ØÖÆÆ÷¡£

> ÖµµÃ×¢ÒâµÄÊÇ£¬[Í¨ÓÃÉèÖÃ](./general_settings.md)´°¿Ú£¨Í¨¹ıgeneral_settings.open()´´½¨£©Ò²ÊÇÓÉÊı¾İ¿ØÖÆÆ÷Éú³ÉµÄ¡£

## Ö§³ÖµÄÀàĞÍ

µ±Ç°Ö§³ÖµÄµ¼³ö±äÁ¿ÀàĞÍÈçÏÂËùÊ¾¡£

`gdscript

#ÒÔÏÂ»®Ïß¿ªÍ·µÄµ¼³ö±äÁ¿½«±»ºöÂÔ¡£
@export var _ignored := 0

#0. ·Ö×é°´Å¥
@export_group( Group 1)

#1. ¹ö¶¯×ÖÄ»µ¥ĞĞ×¢ÊÍ¡£Ãû³ÆĞèÒªÒÔxport_comment_¿ªÍ·¡£
@export var export_comment_1 = ÕâÊÇÒ»¸ö×¢ÊÍ

#2. °´Å¥¡£Ãû³Æ¸ñÊ½Ó¦Îªxport_button_xxx£¬ÆäÖĞxxxÊÇµã»÷°´Å¥Ê±µ÷ÓÃµÄÍ¬Ò»ÎÄ¼şÖĞµÄº¯ÊıÃû³Æ¡£
@export var export_button_xxx = µã»÷ÎÒ

#3. ²¼¶û±äÁ¿¡£
@export var bool_val:bool = false

#4. ÑÕÉ«±äÁ¿¡£
@export var color_val:Color = Color.WHITE

#5. ×Ö·û´®±äÁ¿¡£
@export var string_val:String = "

#6. ¼òµ¥ÕûÊı±äÁ¿¡£
@export var int_val:int = 0

#7. ¼òµ¥¸¡µãÊı±äÁ¿¡£
@export var float_val:float = 0

#8. ´ø·¶Î§µÄÊıÖµ£¨ÕûÊı»ò¸¡µãÊı£©±äÁ¿¡£
@export_range(0.0, 1.0, 0.01) var ranged_number := 0.0

#9. Vector2±äÁ¿¡£
@export var vec2_val:Vector2 = Vector2.ZERO

#10. Ã¶¾ÙÕûÊıÖµ
@export_enum(Ñ¡Ïî1, Ñ¡Ïî2, Ñ¡Ïî3) var enum_val := 0

#11. ²»Ö§³ÖµÄ±äÁ¿½«ÏÔÊ¾ÎªÖ»¶Á×Ö·û´®¡£
@export var node_val:Node

#12. Äú¿ÉÒÔÊ¹ÓÃsetgetº¯Êı¿ØÖÆ·ÃÎÊĞĞÎª¡£
@export var dummy_val:int:
    set(val): pass
    get: return 0

#°´Å¥»Øµ÷º¯Êı
func xxx():
    print(xxx±»µ÷ÓÃ)

`

## Ïà¹ØÎÄ¼ş

panku_console/modules/data_controller/*
