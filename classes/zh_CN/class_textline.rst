:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/TextLine.xml.

.. _class_TextLine:

TextLine
========

**继承：** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

存放一行文本。

.. rst-class:: classref-introduction-group

描述
----

基于 :ref:`TextServer<class_TextServer>` 的抽象，用于处理单行文本。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>`         | :ref:`alignment<class_TextLine_property_alignment>`                         | ``0``     |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`Direction<enum_TextServer_Direction>`                               | :ref:`direction<class_TextLine_property_direction>`                         | ``0``     |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | |bitfield|\<:ref:`JustificationFlag<enum_TextServer_JustificationFlag>`\> | :ref:`flags<class_TextLine_property_flags>`                                 | ``3``     |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`Orientation<enum_TextServer_Orientation>`                           | :ref:`orientation<class_TextLine_property_orientation>`                     | ``0``     |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`                                                   | :ref:`preserve_control<class_TextLine_property_preserve_control>`           | ``false`` |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`                                                   | :ref:`preserve_invalid<class_TextLine_property_preserve_invalid>`           | ``true``  |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>`                   | :ref:`text_overrun_behavior<class_TextLine_property_text_overrun_behavior>` | ``3``     |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`                                                 | :ref:`width<class_TextLine_property_width>`                                 | ``-1.0``  |
   +---------------------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`       | :ref:`add_object<class_TextLine_method_add_object>` **(** :ref:`Variant<class_Variant>` key, :ref:`Vector2<class_Vector2>` size, :ref:`InlineAlignment<enum_@GlobalScope_InlineAlignment>` inline_align=5, :ref:`int<class_int>` length=1, :ref:`float<class_float>` baseline=0.0 **)** |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`       | :ref:`add_string<class_TextLine_method_add_string>` **(** :ref:`String<class_String>` text, :ref:`Font<class_Font>` font, :ref:`int<class_int>` font_size, :ref:`String<class_String>` language="", :ref:`Variant<class_Variant>` meta=null **)**                                       |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                          | :ref:`clear<class_TextLine_method_clear>` **(** **)**                                                                                                                                                                                                                                   |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                          | :ref:`draw<class_TextLine_method_draw>` **(** :ref:`RID<class_RID>` canvas, :ref:`Vector2<class_Vector2>` pos, :ref:`Color<class_Color>` color=Color(1, 1, 1, 1) **)** |const|                                                                                                          |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                          | :ref:`draw_outline<class_TextLine_method_draw_outline>` **(** :ref:`RID<class_RID>` canvas, :ref:`Vector2<class_Vector2>` pos, :ref:`int<class_int>` outline_size=1, :ref:`Color<class_Color>` color=Color(1, 1, 1, 1) **)** |const|                                                    |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`     | :ref:`get_line_ascent<class_TextLine_method_get_line_ascent>` **(** **)** |const|                                                                                                                                                                                                       |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`     | :ref:`get_line_descent<class_TextLine_method_get_line_descent>` **(** **)** |const|                                                                                                                                                                                                     |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`     | :ref:`get_line_underline_position<class_TextLine_method_get_line_underline_position>` **(** **)** |const|                                                                                                                                                                               |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`     | :ref:`get_line_underline_thickness<class_TextLine_method_get_line_underline_thickness>` **(** **)** |const|                                                                                                                                                                             |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`     | :ref:`get_line_width<class_TextLine_method_get_line_width>` **(** **)** |const|                                                                                                                                                                                                         |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Rect2<class_Rect2>`     | :ref:`get_object_rect<class_TextLine_method_get_object_rect>` **(** :ref:`Variant<class_Variant>` key **)** |const|                                                                                                                                                                     |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Array<class_Array>`     | :ref:`get_objects<class_TextLine_method_get_objects>` **(** **)** |const|                                                                                                                                                                                                               |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`RID<class_RID>`         | :ref:`get_rid<class_TextLine_method_get_rid>` **(** **)** |const|                                                                                                                                                                                                                       |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`get_size<class_TextLine_method_get_size>` **(** **)** |const|                                                                                                                                                                                                                     |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`         | :ref:`hit_test<class_TextLine_method_hit_test>` **(** :ref:`float<class_float>` coords **)** |const|                                                                                                                                                                                    |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`       | :ref:`resize_object<class_TextLine_method_resize_object>` **(** :ref:`Variant<class_Variant>` key, :ref:`Vector2<class_Vector2>` size, :ref:`InlineAlignment<enum_@GlobalScope_InlineAlignment>` inline_align=5, :ref:`float<class_float>` baseline=0.0 **)**                           |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                          | :ref:`set_bidi_override<class_TextLine_method_set_bidi_override>` **(** :ref:`Array<class_Array>` override **)**                                                                                                                                                                        |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                          | :ref:`tab_align<class_TextLine_method_tab_align>` **(** :ref:`PackedFloat32Array<class_PackedFloat32Array>` tab_stops **)**                                                                                                                                                             |
   +-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_TextLine_property_alignment:

.. rst-class:: classref-property

:ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **alignment** = ``0``

.. rst-class:: classref-property-setget

- void **set_horizontal_alignment** **(** :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` value **)**
- :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **get_horizontal_alignment** **(** **)**

设置行内的文本对齐方式，始终按照该行为横向的情况设置。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_direction:

.. rst-class:: classref-property

:ref:`Direction<enum_TextServer_Direction>` **direction** = ``0``

.. rst-class:: classref-property-setget

- void **set_direction** **(** :ref:`Direction<enum_TextServer_Direction>` value **)**
- :ref:`Direction<enum_TextServer_Direction>` **get_direction** **(** **)**

文本书写方向。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_flags:

.. rst-class:: classref-property

|bitfield|\<:ref:`JustificationFlag<enum_TextServer_JustificationFlag>`\> **flags** = ``3``

.. rst-class:: classref-property-setget

- void **set_flags** **(** |bitfield|\<:ref:`JustificationFlag<enum_TextServer_JustificationFlag>`\> value **)**
- |bitfield|\<:ref:`JustificationFlag<enum_TextServer_JustificationFlag>`\> **get_flags** **(** **)**

行对齐规则。详细请参阅 :ref:`TextServer<class_TextServer>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_orientation:

.. rst-class:: classref-property

:ref:`Orientation<enum_TextServer_Orientation>` **orientation** = ``0``

.. rst-class:: classref-property-setget

- void **set_orientation** **(** :ref:`Orientation<enum_TextServer_Orientation>` value **)**
- :ref:`Orientation<enum_TextServer_Orientation>` **get_orientation** **(** **)**

文本朝向。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_preserve_control:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **preserve_control** = ``false``

.. rst-class:: classref-property-setget

- void **set_preserve_control** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_preserve_control** **(** **)**

如果设置为 ``true``\ ，则将在文本中显示控制字符。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_preserve_invalid:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **preserve_invalid** = ``true``

.. rst-class:: classref-property-setget

- void **set_preserve_invalid** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_preserve_invalid** **(** **)**

如果设置为 ``true``\ ，则将在文本中显示无效字符。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_text_overrun_behavior:

.. rst-class:: classref-property

:ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>` **text_overrun_behavior** = ``3``

.. rst-class:: classref-property-setget

- void **set_text_overrun_behavior** **(** :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>` value **)**
- :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>` **get_text_overrun_behavior** **(** **)**

设置文本超出文本行的设置宽度时的裁剪行为。有关所有模式的描述，请参阅 :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_property_width:

.. rst-class:: classref-property

:ref:`float<class_float>` **width** = ``-1.0``

.. rst-class:: classref-property-setget

- void **set_width** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_width** **(** **)**

文本行宽。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_TextLine_method_add_object:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **add_object** **(** :ref:`Variant<class_Variant>` key, :ref:`Vector2<class_Vector2>` size, :ref:`InlineAlignment<enum_@GlobalScope_InlineAlignment>` inline_align=5, :ref:`int<class_int>` length=1, :ref:`float<class_float>` baseline=0.0 **)**

向文本缓冲中添加内联对象，\ ``key`` 必须唯一。在文本中，对象使用 ``length`` 个对象替换字符表示。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_add_string:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **add_string** **(** :ref:`String<class_String>` text, :ref:`Font<class_Font>` font, :ref:`int<class_int>` font_size, :ref:`String<class_String>` language="", :ref:`Variant<class_Variant>` meta=null **)**

添加文本区间以及用于绘制的字体。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_clear:

.. rst-class:: classref-method

void **clear** **(** **)**

清除文本行（移除文本和内联对象）。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_draw:

.. rst-class:: classref-method

void **draw** **(** :ref:`RID<class_RID>` canvas, :ref:`Vector2<class_Vector2>` pos, :ref:`Color<class_Color>` color=Color(1, 1, 1, 1) **)** |const|

在画布项中的给定位置绘制文本，颜色为 ``color``\ 。\ ``pos`` 指定的是边界框的左上角。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_draw_outline:

.. rst-class:: classref-method

void **draw_outline** **(** :ref:`RID<class_RID>` canvas, :ref:`Vector2<class_Vector2>` pos, :ref:`int<class_int>` outline_size=1, :ref:`Color<class_Color>` color=Color(1, 1, 1, 1) **)** |const|

在画布项中的给定位置绘制文本，颜色为 ``color``\ 。\ ``pos`` 指定的是边界框的左上角。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_line_ascent:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_line_ascent** **(** **)** |const|

返回该文本的升部（水平排版时为基线上方的像素数，垂直排版时为基线左侧的像素数）。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_line_descent:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_line_descent** **(** **)** |const|

返回该文本的降部（水平排版时为基线下方的像素数，垂直排版时为基线右侧的像素数）。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_line_underline_position:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_line_underline_position** **(** **)** |const|

返回基线下方下划线的像素偏移。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_line_underline_thickness:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_line_underline_thickness** **(** **)** |const|

返回下划线的粗细度。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_line_width:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_line_width** **(** **)** |const|

返回文本的宽度（对于水平排版）或高度（对于垂直排版）。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_object_rect:

.. rst-class:: classref-method

:ref:`Rect2<class_Rect2>` **get_object_rect** **(** :ref:`Variant<class_Variant>` key **)** |const|

返回内联对象的边界矩形。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_objects:

.. rst-class:: classref-method

:ref:`Array<class_Array>` **get_objects** **(** **)** |const|

返回内联对象的数组。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_rid:

.. rst-class:: classref-method

:ref:`RID<class_RID>` **get_rid** **(** **)** |const|

返回 TextServer 缓冲区 RID。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_get_size:

.. rst-class:: classref-method

:ref:`Vector2<class_Vector2>` **get_size** **(** **)** |const|

返回文本边界框的大小。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_hit_test:

.. rst-class:: classref-method

:ref:`int<class_int>` **hit_test** **(** :ref:`float<class_float>` coords **)** |const|

返回基线处指定像素偏移处的文本光标的偏移量。该函数始终返回一个有效位置。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_resize_object:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **resize_object** **(** :ref:`Variant<class_Variant>` key, :ref:`Vector2<class_Vector2>` size, :ref:`InlineAlignment<enum_@GlobalScope_InlineAlignment>` inline_align=5, :ref:`float<class_float>` baseline=0.0 **)**

设置嵌入对象的新大小和对齐方式。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_set_bidi_override:

.. rst-class:: classref-method

void **set_bidi_override** **(** :ref:`Array<class_Array>` override **)**

覆盖用于结构化文本的 BiDi。

覆盖范围应覆盖完整的源文本而没有重叠。BiDi 算法将分别被用于每个范围。

.. rst-class:: classref-item-separator

----

.. _class_TextLine_method_tab_align:

.. rst-class:: classref-method

void **tab_align** **(** :ref:`PackedFloat32Array<class_PackedFloat32Array>` tab_stops **)**

将文本与给定的制表位对齐。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
