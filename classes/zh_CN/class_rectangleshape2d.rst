:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/RectangleShape2D.xml.

.. _class_RectangleShape2D:

RectangleShape2D
================

**继承：** :ref:`Shape2D<class_Shape2D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

2D 矩形，旨在用于物理学。

.. rst-class:: classref-introduction-group

描述
----

2D 矩形，旨在用于物理学。通常用于为 :ref:`CollisionShape2D<class_CollisionShape2D>` 提供形状。

\ **性能：**\ **RectangleShape2D** 可以快速检测碰撞。比 :ref:`CapsuleShape2D<class_CapsuleShape2D>` 快，但比 :ref:`CircleShape2D<class_CircleShape2D>` 慢。

.. rst-class:: classref-introduction-group

教程
----

- `2D Pong 演示 <https://godotengine.org/asset-library/asset/121>`__

- `2D 运动学角色演示 <https://godotengine.org/asset-library/asset/113>`__

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-------------------------------+---------------------------------------------------+---------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`size<class_RectangleShape2D_property_size>` | ``Vector2(20, 20)`` |
   +-------------------------------+---------------------------------------------------+---------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_RectangleShape2D_property_size:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **size** = ``Vector2(20, 20)``

.. rst-class:: classref-property-setget

- void **set_size** **(** :ref:`Vector2<class_Vector2>` value **)**
- :ref:`Vector2<class_Vector2>` **get_size** **(** **)**

该矩形的宽度和高度。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
