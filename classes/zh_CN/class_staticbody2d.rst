:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/StaticBody2D.xml.

.. _class_StaticBody2D:

StaticBody2D
============

**继承：** :ref:`PhysicsBody2D<class_PhysicsBody2D>` **<** :ref:`CollisionObject2D<class_CollisionObject2D>` **<** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**派生：** :ref:`AnimatableBody2D<class_AnimatableBody2D>`

无法被外力移动的 2D 物理物体。手动移动时不会影响路径上的其他物体。

.. rst-class:: classref-introduction-group

描述
----

静态 2D 物理体。无法因外力或接触而移动，但可以通过代码、\ :ref:`AnimationMixer<class_AnimationMixer>`\ （\ :ref:`AnimationMixer.callback_mode_process<class_AnimationMixer_property_callback_mode_process>` 设为 :ref:`AnimationMixer.ANIMATION_CALLBACK_MODE_PROCESS_PHYSICS<class_AnimationMixer_constant_ANIMATION_CALLBACK_MODE_PROCESS_PHYSICS>`\ ）、\ :ref:`RemoteTransform2D<class_RemoteTransform2D>` 等方法手动移动。

\ **StaticBody2D** 发生移动时，是传送到新位置上的，不会影响路径上的其他物理体。如果不想要这样的行为，请改用 :ref:`AnimatableBody2D<class_AnimatableBody2D>`\ 。

\ **StaticBody2D** 常用于完全静态的地板、墙壁等对象，也可以用于传送带、圆形回转平台等移动的表面（使用 :ref:`constant_linear_velocity<class_StaticBody2D_property_constant_linear_velocity>` 和 :ref:`constant_angular_velocity<class_StaticBody2D_property_constant_angular_velocity>`\ ）。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-----------------------------------------------+-----------------------------------------------------------------------------------------+-------------------+
   | :ref:`float<class_float>`                     | :ref:`constant_angular_velocity<class_StaticBody2D_property_constant_angular_velocity>` | ``0.0``           |
   +-----------------------------------------------+-----------------------------------------------------------------------------------------+-------------------+
   | :ref:`Vector2<class_Vector2>`                 | :ref:`constant_linear_velocity<class_StaticBody2D_property_constant_linear_velocity>`   | ``Vector2(0, 0)`` |
   +-----------------------------------------------+-----------------------------------------------------------------------------------------+-------------------+
   | :ref:`PhysicsMaterial<class_PhysicsMaterial>` | :ref:`physics_material_override<class_StaticBody2D_property_physics_material_override>` |                   |
   +-----------------------------------------------+-----------------------------------------------------------------------------------------+-------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_StaticBody2D_property_constant_angular_velocity:

.. rst-class:: classref-property

:ref:`float<class_float>` **constant_angular_velocity** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_constant_angular_velocity** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_constant_angular_velocity** **(** **)**

该物体的恒定角速度。不会旋转该物体，但会影响接触的物体，就好像这个物体正在旋转一样。

.. rst-class:: classref-item-separator

----

.. _class_StaticBody2D_property_constant_linear_velocity:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **constant_linear_velocity** = ``Vector2(0, 0)``

.. rst-class:: classref-property-setget

- void **set_constant_linear_velocity** **(** :ref:`Vector2<class_Vector2>` value **)**
- :ref:`Vector2<class_Vector2>` **get_constant_linear_velocity** **(** **)**

该物体的恒定线速度。不会移动该物体，但会影响接触的物体，就好像这个物体正在移动一样。

.. rst-class:: classref-item-separator

----

.. _class_StaticBody2D_property_physics_material_override:

.. rst-class:: classref-property

:ref:`PhysicsMaterial<class_PhysicsMaterial>` **physics_material_override**

.. rst-class:: classref-property-setget

- void **set_physics_material_override** **(** :ref:`PhysicsMaterial<class_PhysicsMaterial>` value **)**
- :ref:`PhysicsMaterial<class_PhysicsMaterial>` **get_physics_material_override** **(** **)**

物体的物理材质。

如果为该属性指定了一种材质，则将使用该材质代替任何其他物理材质，例如继承的材质。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
