:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/InputEventMagnifyGesture.xml.

.. _class_InputEventMagnifyGesture:

InputEventMagnifyGesture
========================

**继承：** :ref:`InputEventGesture<class_InputEventGesture>` **<** :ref:`InputEventWithModifiers<class_InputEventWithModifiers>` **<** :ref:`InputEventFromWindow<class_InputEventFromWindow>` **<** :ref:`InputEvent<class_InputEvent>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

代表放大触摸手势。

.. rst-class:: classref-introduction-group

描述
----

存储放大触摸手势的系数。通常用户在触摸屏上将双指捏合，就执行了放大手势，可用于缩放。

\ **注意：**\ 在 Android 上，这需要启用 :ref:`ProjectSettings.input_devices/pointing/android/enable_pan_and_scale_gestures<class_ProjectSettings_property_input_devices/pointing/android/enable_pan_and_scale_gestures>` 项目设置。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`使用 InputEvent <../tutorials/inputs/inputevent>`

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------+---------------------------------------------------------------+---------+
   | :ref:`float<class_float>` | :ref:`factor<class_InputEventMagnifyGesture_property_factor>` | ``1.0`` |
   +---------------------------+---------------------------------------------------------------+---------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_InputEventMagnifyGesture_property_factor:

.. rst-class:: classref-property

:ref:`float<class_float>` **factor** = ``1.0``

.. rst-class:: classref-property-setget

- void **set_factor** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_factor** **(** **)**

事件的量（或增量）。这个值越接近 ``1.0``\ ，手势执行地越快。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
