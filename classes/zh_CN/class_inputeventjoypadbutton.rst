:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/InputEventJoypadButton.xml.

.. _class_InputEventJoypadButton:

InputEventJoypadButton
======================

**继承：** :ref:`InputEvent<class_InputEvent>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

代表按下或松开的游戏手柄按钮。

.. rst-class:: classref-introduction-group

描述
----

游戏手柄按钮的输入事件类型。对于游戏手柄模拟摇杆和操纵杆，请参阅 :ref:`InputEventJoypadMotion<class_InputEventJoypadMotion>`\ 。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`使用 InputEvent <../tutorials/inputs/inputevent>`

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-----------------------------------------------+-------------------------------------------------------------------------+-----------+
   | :ref:`JoyButton<enum_@GlobalScope_JoyButton>` | :ref:`button_index<class_InputEventJoypadButton_property_button_index>` | ``0``     |
   +-----------------------------------------------+-------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`                       | :ref:`pressed<class_InputEventJoypadButton_property_pressed>`           | ``false`` |
   +-----------------------------------------------+-------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`                     | :ref:`pressure<class_InputEventJoypadButton_property_pressure>`         | ``0.0``   |
   +-----------------------------------------------+-------------------------------------------------------------------------+-----------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_InputEventJoypadButton_property_button_index:

.. rst-class:: classref-property

:ref:`JoyButton<enum_@GlobalScope_JoyButton>` **button_index** = ``0``

.. rst-class:: classref-property-setget

- void **set_button_index** **(** :ref:`JoyButton<enum_@GlobalScope_JoyButton>` value **)**
- :ref:`JoyButton<enum_@GlobalScope_JoyButton>` **get_button_index** **(** **)**

按钮标识符。\ :ref:`JoyButton<enum_@GlobalScope_JoyButton>` 按钮常量之一。

.. rst-class:: classref-item-separator

----

.. _class_InputEventJoypadButton_property_pressed:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **pressed** = ``false``

.. rst-class:: classref-property-setget

- void **set_pressed** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_pressed** **(** **)**

如果为 ``true``\ ，按钮的状态被按下。如果为 ``false``\ ，按钮的状态被释放。

.. rst-class:: classref-item-separator

----

.. _class_InputEventJoypadButton_property_pressure:

.. rst-class:: classref-property

:ref:`float<class_float>` **pressure** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_pressure** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_pressure** **(** **)**

如果控制器支持，则表示用户用手指在按钮上施加的压力。范围从 ``0`` 到 ``1``\ 。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
