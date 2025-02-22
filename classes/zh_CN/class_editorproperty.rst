:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/EditorProperty.xml.

.. _class_EditorProperty:

EditorProperty
==============

**继承：** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

用于编辑属性的自定义控件，可以添加到 :ref:`EditorInspector<class_EditorInspector>` 中。

.. rst-class:: classref-introduction-group

描述
----

用于编辑属性的自定义控件，可以添加到 :ref:`EditorInspector<class_EditorInspector>` 中。通过 :ref:`EditorInspectorPlugin<class_EditorInspectorPlugin>` 添加。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`checkable<class_EditorProperty_property_checkable>`       | ``false`` |
   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`checked<class_EditorProperty_property_checked>`           | ``false`` |
   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`deletable<class_EditorProperty_property_deletable>`       | ``false`` |
   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`draw_warning<class_EditorProperty_property_draw_warning>` | ``false`` |
   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`keying<class_EditorProperty_property_keying>`             | ``false`` |
   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`String<class_String>` | :ref:`label<class_EditorProperty_property_label>`               | ``""``    |
   +-----------------------------+-----------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`read_only<class_EditorProperty_property_read_only>`       | ``false`` |
   +-----------------------------+-----------------------------------------------------------------+-----------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                | :ref:`_set_read_only<class_EditorProperty_private_method__set_read_only>` **(** :ref:`bool<class_bool>` read_only **)** |virtual|                                                                                                                  |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                | :ref:`_update_property<class_EditorProperty_private_method__update_property>` **(** **)** |virtual|                                                                                                                                                |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                | :ref:`add_focusable<class_EditorProperty_method_add_focusable>` **(** :ref:`Control<class_Control>` control **)**                                                                                                                                  |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                | :ref:`emit_changed<class_EditorProperty_method_emit_changed>` **(** :ref:`StringName<class_StringName>` property, :ref:`Variant<class_Variant>` value, :ref:`StringName<class_StringName>` field=&"", :ref:`bool<class_bool>` changing=false **)** |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Object<class_Object>`         | :ref:`get_edited_object<class_EditorProperty_method_get_edited_object>` **(** **)**                                                                                                                                                                |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`StringName<class_StringName>` | :ref:`get_edited_property<class_EditorProperty_method_get_edited_property>` **(** **)** |const|                                                                                                                                                    |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                | :ref:`set_bottom_editor<class_EditorProperty_method_set_bottom_editor>` **(** :ref:`Control<class_Control>` editor **)**                                                                                                                           |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                | :ref:`update_property<class_EditorProperty_method_update_property>` **(** **)**                                                                                                                                                                    |
   +-------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

信号
----

.. _class_EditorProperty_signal_multiple_properties_changed:

.. rst-class:: classref-signal

**multiple_properties_changed** **(** :ref:`PackedStringArray<class_PackedStringArray>` properties, :ref:`Array<class_Array>` value **)**

如果想要同时修改多个属性，请发出它。如果属性是通过 :ref:`EditorInspectorPlugin._parse_property<class_EditorInspectorPlugin_private_method__parse_property>` 添加的，请勿使用。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_object_id_selected:

.. rst-class:: classref-signal

**object_id_selected** **(** :ref:`StringName<class_StringName>` property, :ref:`int<class_int>` id **)**

子检查器会使用。如果选择的是对象 ID，则触发。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_can_revert_changed:

.. rst-class:: classref-signal

**property_can_revert_changed** **(** :ref:`StringName<class_StringName>` property, :ref:`bool<class_bool>` can_revert **)**

当属性的可恢复性（即，它是否具有非默认值并因此显示为带有恢复图标）发生变化时发出。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_changed:

.. rst-class:: classref-signal

**property_changed** **(** :ref:`StringName<class_StringName>` property, :ref:`Variant<class_Variant>` value, :ref:`StringName<class_StringName>` field, :ref:`bool<class_bool>` changing **)**

不要手动触发，使用 :ref:`emit_changed<class_EditorProperty_method_emit_changed>` 方法代替。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_checked:

.. rst-class:: classref-signal

**property_checked** **(** :ref:`StringName<class_StringName>` property, :ref:`bool<class_bool>` checked **)**

勾选某个属性时发出。内部使用。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_deleted:

.. rst-class:: classref-signal

**property_deleted** **(** :ref:`StringName<class_StringName>` property **)**

删除某个属性时发出。内部使用。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_keyed:

.. rst-class:: classref-signal

**property_keyed** **(** :ref:`StringName<class_StringName>` property **)**

如果你想将此值添加这个值为动画键，请触发它（首先检查是否启用了键控）。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_keyed_with_value:

.. rst-class:: classref-signal

**property_keyed_with_value** **(** :ref:`StringName<class_StringName>` property, :ref:`Variant<class_Variant>` value **)**

如果你想用一个单一的值来键入一个属性，请触发它。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_property_pinned:

.. rst-class:: classref-signal

**property_pinned** **(** :ref:`StringName<class_StringName>` property, :ref:`bool<class_bool>` pinned **)**

如果想要对某个属性进行标记（或者取消标记），让它无论是否与默认值相等都进行保存，请发出它。

默认值指节点刚刚实例化后属性的取值，可以来自继承/实例化链上的祖先场景、脚本或内置类。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_resource_selected:

.. rst-class:: classref-signal

**resource_selected** **(** :ref:`String<class_String>` path, :ref:`Resource<class_Resource>` resource **)**

如果你想编辑一个子资源，请将此信号与资源一起发出。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_signal_selected:

.. rst-class:: classref-signal

**selected** **(** :ref:`String<class_String>` path, :ref:`int<class_int>` focusable_idx **)**

选择时触发。内部使用。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_EditorProperty_property_checkable:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **checkable** = ``false``

.. rst-class:: classref-property-setget

- void **set_checkable** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_checkable** **(** **)**

用于检查器，该属性可勾选时设置为 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_property_checked:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **checked** = ``false``

.. rst-class:: classref-property-setget

- void **set_checked** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_checked** **(** **)**

用于检查器，该属性已勾选时设置为 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_property_deletable:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **deletable** = ``false``

.. rst-class:: classref-property-setget

- void **set_deletable** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_deletable** **(** **)**

用于检查器，该属性可以被用户删除时设置为 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_property_draw_warning:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **draw_warning** = ``false``

.. rst-class:: classref-property-setget

- void **set_draw_warning** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_draw_warning** **(** **)**

用于检查器，该属性用编辑器主题的警告色绘制时设置为 ``true``\ 。用于可编辑子节点的属性。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_property_keying:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **keying** = ``false``

.. rst-class:: classref-property-setget

- void **set_keying** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_keying** **(** **)**

用于检查器，该属性可以被添加为动画关键帧时设置为 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_property_label:

.. rst-class:: classref-property

:ref:`String<class_String>` **label** = ``""``

.. rst-class:: classref-property-setget

- void **set_label** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_label** **(** **)**

设置此属性可改变标签（如果你想显示标签）。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_property_read_only:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **read_only** = ``false``

.. rst-class:: classref-property-setget

- void **set_read_only** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_read_only** **(** **)**

用于检查器，该属性为只读时设置为 ``true``\ 。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_EditorProperty_private_method__set_read_only:

.. rst-class:: classref-method

void **_set_read_only** **(** :ref:`bool<class_bool>` read_only **)** |virtual|

当属性的只读状态被改变时被调用。它可用于将自定义控件改变为只读或可修改的状态。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_private_method__update_property:

.. rst-class:: classref-method

void **_update_property** **(** **)** |virtual|

当这个虚函数被调用时，你必须更新你的编辑器。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_method_add_focusable:

.. rst-class:: classref-method

void **add_focusable** **(** :ref:`Control<class_Control>` control **)**

如果添加的任何控件可以获得键盘焦点，将其添加到此处。这样可以确保在检查器被刷新时恢复焦点。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_method_emit_changed:

.. rst-class:: classref-method

void **emit_changed** **(** :ref:`StringName<class_StringName>` property, :ref:`Variant<class_Variant>` value, :ref:`StringName<class_StringName>` field=&"", :ref:`bool<class_bool>` changing=false **)**

如果一个或几个属性发生了变化，必然会调用这个函数。\ ``field`` 用于你的编辑器可以单独修改字段的情况（例如，Vector3.x）。\ ``changing`` 参数可以避免编辑器请求刷新该属性（如果不确定，请保留为 ``false``\ ）。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_method_get_edited_object:

.. rst-class:: classref-method

:ref:`Object<class_Object>` **get_edited_object** **(** **)**

获取被编辑的对象。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_method_get_edited_property:

.. rst-class:: classref-method

:ref:`StringName<class_StringName>` **get_edited_property** **(** **)** |const|

获取被编辑的属性。如果你的编辑器适用于单个属性（通过 :ref:`EditorInspectorPlugin._parse_property<class_EditorInspectorPlugin_private_method__parse_property>` 添加），则返回该属性。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_method_set_bottom_editor:

.. rst-class:: classref-method

void **set_bottom_editor** **(** :ref:`Control<class_Control>` editor **)**

将 ``editor`` 控件放在属性标签的下方。该控件必须事先用 :ref:`Node.add_child<class_Node_method_add_child>` 添加。

.. rst-class:: classref-item-separator

----

.. _class_EditorProperty_method_update_property:

.. rst-class:: classref-method

void **update_property** **(** **)**

强制刷新属性显示。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
