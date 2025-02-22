:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/VisualShaderNodeVectorBase.xml.

.. _class_VisualShaderNodeVectorBase:

VisualShaderNodeVectorBase
==========================

**继承：** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

**派生：** :ref:`VisualShaderNodeFaceForward<class_VisualShaderNodeFaceForward>`, :ref:`VisualShaderNodeVectorCompose<class_VisualShaderNodeVectorCompose>`, :ref:`VisualShaderNodeVectorDecompose<class_VisualShaderNodeVectorDecompose>`, :ref:`VisualShaderNodeVectorDistance<class_VisualShaderNodeVectorDistance>`, :ref:`VisualShaderNodeVectorFunc<class_VisualShaderNodeVectorFunc>`, :ref:`VisualShaderNodeVectorLen<class_VisualShaderNodeVectorLen>`, :ref:`VisualShaderNodeVectorOp<class_VisualShaderNodeVectorOp>`, :ref:`VisualShaderNodeVectorRefract<class_VisualShaderNodeVectorRefract>`

在可视化着色器图中执行向量运算的基础类型节点。

.. rst-class:: classref-introduction-group

描述
----

这是一个抽象类。可进行的运算描述见派生类。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-------------------------------------------------------+-------------------------------------------------------------------+-------+
   | :ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` | :ref:`op_type<class_VisualShaderNodeVectorBase_property_op_type>` | ``1`` |
   +-------------------------------------------------------+-------------------------------------------------------------------+-------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

枚举
----

.. _enum_VisualShaderNodeVectorBase_OpType:

.. rst-class:: classref-enumeration

enum **OpType**:

.. _class_VisualShaderNodeVectorBase_constant_OP_TYPE_VECTOR_2D:

.. rst-class:: classref-enumeration-constant

:ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` **OP_TYPE_VECTOR_2D** = ``0``

2D 向量类型。

.. _class_VisualShaderNodeVectorBase_constant_OP_TYPE_VECTOR_3D:

.. rst-class:: classref-enumeration-constant

:ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` **OP_TYPE_VECTOR_3D** = ``1``

3D向量类型。

.. _class_VisualShaderNodeVectorBase_constant_OP_TYPE_VECTOR_4D:

.. rst-class:: classref-enumeration-constant

:ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` **OP_TYPE_VECTOR_4D** = ``2``

4D 向量类型。

.. _class_VisualShaderNodeVectorBase_constant_OP_TYPE_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` **OP_TYPE_MAX** = ``3``

代表 :ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` 枚举的大小。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_VisualShaderNodeVectorBase_property_op_type:

.. rst-class:: classref-property

:ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` **op_type** = ``1``

.. rst-class:: classref-property-setget

- void **set_op_type** **(** :ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` value **)**
- :ref:`OpType<enum_VisualShaderNodeVectorBase_OpType>` **get_op_type** **(** **)**

要进行运算的向量类型。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
