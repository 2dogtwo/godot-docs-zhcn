:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/Button.xml.

.. _class_Button:

Button
======

**继承：** :ref:`BaseButton<class_BaseButton>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**派生：** :ref:`CheckBox<class_CheckBox>`, :ref:`CheckButton<class_CheckButton>`, :ref:`ColorPickerButton<class_ColorPickerButton>`, :ref:`MenuButton<class_MenuButton>`, :ref:`OptionButton<class_OptionButton>`

按钮，支持主题，能够包含文本和图标。

.. rst-class:: classref-introduction-group

描述
----

**Button** 是标准的主题按钮，可以包含文字和图标，显示样式会根据当前的 :ref:`Theme<class_Theme>` 改变。

\ **示例：通过代码创建按钮并指定在按下时的动作**\ 


.. tabs::

 .. code-tab:: gdscript

    func _ready():
        var button = Button.new()
        button.text = "Click me"
        button.pressed.connect(self._button_pressed)
        add_child(button)
    
    func _button_pressed():
        print("Hello world!")

 .. code-tab:: csharp

    public override void _Ready()
    {
        var button = new Button();
        button.Text = "Click me";
        button.Pressed += ButtonPressed;
        AddChild(button);
    }
    
    private void ButtonPressed()
    {
        GD.Print("Hello world!");
    }



另请参阅 :ref:`BaseButton<class_BaseButton>`\ ，其中包含与此节点相关联的通用属性和方法。

\ **注意：**\ 按钮不处理触摸输入，因此不支持多点触控，因为模拟鼠标在给定时间只能按下一个按钮。请用 :ref:`TouchScreenButton<class_TouchScreenButton>` 制作触发游戏移动或动作的按钮。

.. rst-class:: classref-introduction-group

教程
----

- `2D Dodge The Creeps 演示 <https://godotengine.org/asset-library/asset/515>`__

- `操作系统测试演示 <https://godotengine.org/asset-library/asset/677>`__

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` | :ref:`alignment<class_Button_property_alignment>`                             | ``1``     |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`                                           | :ref:`clip_text<class_Button_property_clip_text>`                             | ``false`` |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`                                           | :ref:`expand_icon<class_Button_property_expand_icon>`                         | ``false`` |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`                                           | :ref:`flat<class_Button_property_flat>`                                       | ``false`` |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`Texture2D<class_Texture2D>`                                 | :ref:`icon<class_Button_property_icon>`                                       |           |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` | :ref:`icon_alignment<class_Button_property_icon_alignment>`                   | ``0``     |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`String<class_String>`                                       | :ref:`language<class_Button_property_language>`                               | ``""``    |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`String<class_String>`                                       | :ref:`text<class_Button_property_text>`                                       | ``""``    |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`TextDirection<enum_Control_TextDirection>`                  | :ref:`text_direction<class_Button_property_text_direction>`                   | ``0``     |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>`           | :ref:`text_overrun_behavior<class_Button_property_text_overrun_behavior>`     | ``0``     |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+
   | :ref:`VerticalAlignment<enum_@GlobalScope_VerticalAlignment>`     | :ref:`vertical_icon_alignment<class_Button_property_vertical_icon_alignment>` | ``1``     |
   +-------------------------------------------------------------------+-------------------------------------------------------------------------------+-----------+

.. rst-class:: classref-reftable-group

主题属性
--------

.. table::
   :widths: auto

   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_color<class_Button_theme_color_font_color>`                             | ``Color(0.875, 0.875, 0.875, 1)``   |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_disabled_color<class_Button_theme_color_font_disabled_color>`           | ``Color(0.875, 0.875, 0.875, 0.5)`` |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_focus_color<class_Button_theme_color_font_focus_color>`                 | ``Color(0.95, 0.95, 0.95, 1)``      |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_hover_color<class_Button_theme_color_font_hover_color>`                 | ``Color(0.95, 0.95, 0.95, 1)``      |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_hover_pressed_color<class_Button_theme_color_font_hover_pressed_color>` | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_outline_color<class_Button_theme_color_font_outline_color>`             | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`font_pressed_color<class_Button_theme_color_font_pressed_color>`             | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`icon_disabled_color<class_Button_theme_color_icon_disabled_color>`           | ``Color(1, 1, 1, 0.4)``             |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`icon_focus_color<class_Button_theme_color_icon_focus_color>`                 | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`icon_hover_color<class_Button_theme_color_icon_hover_color>`                 | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`icon_hover_pressed_color<class_Button_theme_color_icon_hover_pressed_color>` | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`icon_normal_color<class_Button_theme_color_icon_normal_color>`               | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Color<class_Color>`         | :ref:`icon_pressed_color<class_Button_theme_color_icon_pressed_color>`             | ``Color(1, 1, 1, 1)``               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`int<class_int>`             | :ref:`h_separation<class_Button_theme_constant_h_separation>`                      | ``4``                               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`int<class_int>`             | :ref:`icon_max_width<class_Button_theme_constant_icon_max_width>`                  | ``0``                               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`int<class_int>`             | :ref:`outline_size<class_Button_theme_constant_outline_size>`                      | ``0``                               |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Font<class_Font>`           | :ref:`font<class_Button_theme_font_font>`                                          |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`int<class_int>`             | :ref:`font_size<class_Button_theme_font_size_font_size>`                           |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`Texture2D<class_Texture2D>` | :ref:`icon<class_Button_theme_icon_icon>`                                          |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`disabled<class_Button_theme_style_disabled>`                                 |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`disabled_mirrored<class_Button_theme_style_disabled_mirrored>`               |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`focus<class_Button_theme_style_focus>`                                       |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`hover<class_Button_theme_style_hover>`                                       |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`hover_mirrored<class_Button_theme_style_hover_mirrored>`                     |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`hover_pressed<class_Button_theme_style_hover_pressed>`                       |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`hover_pressed_mirrored<class_Button_theme_style_hover_pressed_mirrored>`     |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`normal<class_Button_theme_style_normal>`                                     |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`normal_mirrored<class_Button_theme_style_normal_mirrored>`                   |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`pressed<class_Button_theme_style_pressed>`                                   |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+
   | :ref:`StyleBox<class_StyleBox>`   | :ref:`pressed_mirrored<class_Button_theme_style_pressed_mirrored>`                 |                                     |
   +-----------------------------------+------------------------------------------------------------------------------------+-------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_Button_property_alignment:

.. rst-class:: classref-property

:ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **alignment** = ``1``

.. rst-class:: classref-property-setget

- void **set_text_alignment** **(** :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` value **)**
- :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **get_text_alignment** **(** **)**

按钮文本的文本对齐策略，使用 :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` 常量之一。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_clip_text:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **clip_text** = ``false``

.. rst-class:: classref-property-setget

- void **set_clip_text** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_clip_text** **(** **)**

当此属性被启用时，过大而无法容纳按钮的文本会被剪掉，当被禁用时，按钮将始终有足够的宽度来容纳文本。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_expand_icon:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **expand_icon** = ``false``

.. rst-class:: classref-property-setget

- void **set_expand_icon** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_expand_icon** **(** **)**

启用后，将在保持按钮图标长宽比的前提下对该图标进行扩展/收缩，从而适应按钮的大小。另见 :ref:`icon_max_width<class_Button_theme_constant_icon_max_width>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_flat:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **flat** = ``false``

.. rst-class:: classref-property-setget

- void **set_flat** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_flat** **(** **)**

平面按钮不显示装饰。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_icon:

.. rst-class:: classref-property

:ref:`Texture2D<class_Texture2D>` **icon**

.. rst-class:: classref-property-setget

- void **set_button_icon** **(** :ref:`Texture2D<class_Texture2D>` value **)**
- :ref:`Texture2D<class_Texture2D>` **get_button_icon** **(** **)**

按钮的图标，如果文本存在，则图标将被放置在文本之前。

要编辑图标的边距和间距，请使用 :ref:`h_separation<class_Button_theme_constant_h_separation>` 主题属性，和所用 :ref:`StyleBox<class_StyleBox>` 的 ``content_margin_*`` 属性。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_icon_alignment:

.. rst-class:: classref-property

:ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **icon_alignment** = ``0``

.. rst-class:: classref-property-setget

- void **set_icon_alignment** **(** :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` value **)**
- :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **get_icon_alignment** **(** **)**

指定图标在按钮上水平对齐的方式应该为左对齐、右对齐还是居中对齐。请使用与文本对齐相同的 :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` 常量。如果水平居中并且垂直居中，则文本将被绘制在图标之上。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_language:

.. rst-class:: classref-property

:ref:`String<class_String>` **language** = ``""``

.. rst-class:: classref-property-setget

- void **set_language** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_language** **(** **)**

语言代码，用于断行和文本塑形算法，如果留空则使用当前区域设置。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_text:

.. rst-class:: classref-property

:ref:`String<class_String>` **text** = ``""``

.. rst-class:: classref-property-setget

- void **set_text** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_text** **(** **)**

该按钮的文本，将显示在按钮的区域内。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_text_direction:

.. rst-class:: classref-property

:ref:`TextDirection<enum_Control_TextDirection>` **text_direction** = ``0``

.. rst-class:: classref-property-setget

- void **set_text_direction** **(** :ref:`TextDirection<enum_Control_TextDirection>` value **)**
- :ref:`TextDirection<enum_Control_TextDirection>` **get_text_direction** **(** **)**

基础文本书写方向。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_text_overrun_behavior:

.. rst-class:: classref-property

:ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>` **text_overrun_behavior** = ``0``

.. rst-class:: classref-property-setget

- void **set_text_overrun_behavior** **(** :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>` value **)**
- :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>` **get_text_overrun_behavior** **(** **)**

设置文本超出节点的边界矩形时的裁剪行为。有关所有模式的描述，请参阅 :ref:`OverrunBehavior<enum_TextServer_OverrunBehavior>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_property_vertical_icon_alignment:

.. rst-class:: classref-property

:ref:`VerticalAlignment<enum_@GlobalScope_VerticalAlignment>` **vertical_icon_alignment** = ``1``

.. rst-class:: classref-property-setget

- void **set_vertical_icon_alignment** **(** :ref:`VerticalAlignment<enum_@GlobalScope_VerticalAlignment>` value **)**
- :ref:`VerticalAlignment<enum_@GlobalScope_VerticalAlignment>` **get_vertical_icon_alignment** **(** **)**

指定图标在按钮上垂直对齐的方式应该为顶端对齐、底部对齐还是居中对齐。请使用与文本对齐相同的 :ref:`VerticalAlignment<enum_@GlobalScope_VerticalAlignment>` 常量。如果水平居中并且垂直居中，则文本将被绘制在图标之上。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

主题属性说明
------------

.. _class_Button_theme_color_font_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_color** = ``Color(0.875, 0.875, 0.875, 1)``

该 **Button** 的默认文本 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_font_disabled_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_disabled_color** = ``Color(0.875, 0.875, 0.875, 0.5)``

该 **Button** 处于禁用状态时，使用的文本 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_font_focus_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_focus_color** = ``Color(0.95, 0.95, 0.95, 1)``

该 **Button** 处于聚焦状态时，使用的文本 :ref:`Color<class_Color>`\ 。只替换该按钮的正常文本颜色。禁用、悬停、按下状态优先于这个颜色。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_font_hover_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_hover_color** = ``Color(0.95, 0.95, 0.95, 1)``

该 **Button** 处于悬停状态时，使用的文本 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_font_hover_pressed_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_hover_pressed_color** = ``Color(1, 1, 1, 1)``

该 **Button** 处于悬停并按下状态时，使用的文本 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_font_outline_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_outline_color** = ``Color(1, 1, 1, 1)``

该 **Button** 的文本轮廓的色调。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_font_pressed_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **font_pressed_color** = ``Color(1, 1, 1, 1)``

该 **Button** 处于按下状态时，使用的文本 :ref:`Color<class_Color>` 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_icon_disabled_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **icon_disabled_color** = ``Color(1, 1, 1, 0.4)``

该 **Button** 处于禁用状态时，使用的图标调制 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_icon_focus_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **icon_focus_color** = ``Color(1, 1, 1, 1)``

该 **Button** 处于聚焦状态时，使用的图标调制 :ref:`Color<class_Color>`\ 。仅替换该按钮的正常调制颜色。禁用、悬停和按下状态优先于这个颜色。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_icon_hover_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **icon_hover_color** = ``Color(1, 1, 1, 1)``

该 **Button** 处于悬停状态时，使用的图标调制\ :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_icon_hover_pressed_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **icon_hover_pressed_color** = ``Color(1, 1, 1, 1)``

该 **Button** 处于悬停并按下按下状态时，使用的图标调制 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_icon_normal_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **icon_normal_color** = ``Color(1, 1, 1, 1)``

该 **Button** 的默认图标调制 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_color_icon_pressed_color:

.. rst-class:: classref-themeproperty

:ref:`Color<class_Color>` **icon_pressed_color** = ``Color(1, 1, 1, 1)``

该 **Button** 处于按下状态时，使用的图标调制 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_constant_h_separation:

.. rst-class:: classref-themeproperty

:ref:`int<class_int>` **h_separation** = ``4``

**Button** 的图标和文本之间的水平间距。使用时会将负值当作 ``0``\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_constant_icon_max_width:

.. rst-class:: classref-themeproperty

:ref:`int<class_int>` **icon_max_width** = ``0``

**Button** 图标的最大允许宽度。如果 :ref:`expand_icon<class_Button_property_expand_icon>` 为 ``true``\ ，则该限制适用于图标的默认大小或扩展大小。高度将根据图标的比例进行调整。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_constant_outline_size:

.. rst-class:: classref-themeproperty

:ref:`int<class_int>` **outline_size** = ``0``

文字轮廓的大小。

\ **注意：**\ 如果使用启用了 :ref:`FontFile.multichannel_signed_distance_field<class_FontFile_property_multichannel_signed_distance_field>` 的字体，其 :ref:`FontFile.msdf_pixel_range<class_FontFile_property_msdf_pixel_range>` 必须至少设置为 :ref:`outline_size<class_Button_theme_constant_outline_size>` 的\ *两倍*\ ，轮廓渲染才能看起来正确。否则，轮廓可能会比预期的更早被切断。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_font_font:

.. rst-class:: classref-themeproperty

:ref:`Font<class_Font>` **font**

该 **Button** 文本的 :ref:`Font<class_Font>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_font_size_font_size:

.. rst-class:: classref-themeproperty

:ref:`int<class_int>` **font_size**

该 **Button** 文本的字体大小。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_icon_icon:

.. rst-class:: classref-themeproperty

:ref:`Texture2D<class_Texture2D>` **icon**

该 **Button** 的默认图标。仅在未指定 :ref:`icon<class_Button_property_icon>` 时显示。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_disabled:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **disabled**

该 **Button** 处于禁用状态时使用的 :ref:`StyleBox<class_StyleBox>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_disabled_mirrored:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **disabled_mirrored**

该 **Button** 处于禁用状态时使用的 :ref:`StyleBox<class_StyleBox>`\ （用于从右至左布局）。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_focus:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **focus**

该 **Button** 处于聚焦状态时使用的 :ref:`StyleBox<class_StyleBox>`\ 。\ :ref:`focus<class_Button_theme_style_focus>` :ref:`StyleBox<class_StyleBox>` 显示在基础 :ref:`StyleBox<class_StyleBox>` *之上*\ ，所以应该使用部分透明的 :ref:`StyleBox<class_StyleBox>`\ ，确保基础 :ref:`StyleBox<class_StyleBox>` 仍然可见。代表轮廓或下划线的 :ref:`StyleBox<class_StyleBox>` 可以很好地实现这个目的。要禁用聚焦的视觉效果，请指定 :ref:`StyleBoxEmpty<class_StyleBoxEmpty>` 资源。请注意，禁用聚焦的视觉效果会影响使用键盘/手柄进行导航的可用性，所以出于可访问性的原因，不建议这样做。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_hover:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **hover**

该 **Button** 处于悬停状态时使用的 :ref:`StyleBox<class_StyleBox>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_hover_mirrored:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **hover_mirrored**

该 **Button** 处于悬停状态时使用的 :ref:`StyleBox<class_StyleBox>`\ （用于从右至左布局）。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_hover_pressed:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **hover_pressed**

该 **Button** 同时处于按下和悬停状态时使用的 :ref:`StyleBox<class_StyleBox>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_hover_pressed_mirrored:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **hover_pressed_mirrored**

该 **Button** 同时处于按下和悬停状态时使用的 :ref:`StyleBox<class_StyleBox>`\ （用于从右至左布局）。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_normal:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **normal**

该 **Button** 的默认 :ref:`StyleBox<class_StyleBox>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_normal_mirrored:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **normal_mirrored**

该 **Button** 的默认 :ref:`StyleBox<class_StyleBox>`\ （用于从右至左布局）。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_pressed:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **pressed**

该 **Button** 处于按下状态时使用的 :ref:`StyleBox<class_StyleBox>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Button_theme_style_pressed_mirrored:

.. rst-class:: classref-themeproperty

:ref:`StyleBox<class_StyleBox>` **pressed_mirrored**

该 **Button** 处于按下状态时使用的 :ref:`StyleBox<class_StyleBox>`\ （用于从右至左布局）。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
