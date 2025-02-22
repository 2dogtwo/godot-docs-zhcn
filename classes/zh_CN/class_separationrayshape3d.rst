:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/SeparationRayShape3D.xml.

.. _class_SeparationRayShape3D:

SeparationRayShape3D
====================

**继承：** :ref:`Shape3D<class_Shape3D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

用于物理碰撞的 3D 射线形状，会尝试将自己与其他碰撞体分开。

.. rst-class:: classref-introduction-group

描述
----

3D 射线形状，旨在用于物理。通常用来为 :ref:`CollisionShape3D<class_CollisionShape3D>` 提供形状。\ **SeparationRayShape3D** 与某个对象发生碰撞时，会尝试将其端点移动至碰撞点，来将自己与该对象分离。例如，角色旁边的 **SeparationRayShape3D** 可以让角色在接触楼梯时立即向上移动。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------+---------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>` | :ref:`length<class_SeparationRayShape3D_property_length>`                 | ``1.0``   |
   +---------------------------+---------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`   | :ref:`slide_on_slope<class_SeparationRayShape3D_property_slide_on_slope>` | ``false`` |
   +---------------------------+---------------------------------------------------------------------------+-----------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_SeparationRayShape3D_property_length:

.. rst-class:: classref-property

:ref:`float<class_float>` **length** = ``1.0``

.. rst-class:: classref-property-setget

- void **set_length** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_length** **(** **)**

射线的长度。

.. rst-class:: classref-item-separator

----

.. _class_SeparationRayShape3D_property_slide_on_slope:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **slide_on_slope** = ``false``

.. rst-class:: classref-property-setget

- void **set_slide_on_slope** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_slide_on_slope** **(** **)**

如果为 ``false``\ （默认值），则形状始终分离，并返回一条沿其自身方向的法线。

如果为 ``true``\ ，则该形状可以返回正确的法线，并在任何方向上分离，允许在斜坡上滑动。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
