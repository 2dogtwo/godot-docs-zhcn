:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/MissingResource.xml.

.. _class_MissingResource:

MissingResource
===============

**继承：** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

编辑器内部类，用于保存未知资源的数据。

.. rst-class:: classref-introduction-group

描述
----

这是编辑器内部类，用于保存未知类型资源的数据（该类型很有可能是由扩展提供的，而该扩展未加载）。无法手动实例化或放置在场景中。如果你不知道这是什么，请忽略它。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-----------------------------+----------------------------------------------------------------------------------+
   | :ref:`String<class_String>` | :ref:`original_class<class_MissingResource_property_original_class>`             |
   +-----------------------------+----------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`     | :ref:`recording_properties<class_MissingResource_property_recording_properties>` |
   +-----------------------------+----------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_MissingResource_property_original_class:

.. rst-class:: classref-property

:ref:`String<class_String>` **original_class**

.. rst-class:: classref-property-setget

- void **set_original_class** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_original_class** **(** **)**

返回这个资源原本的类名。

.. rst-class:: classref-item-separator

----

.. _class_MissingResource_property_recording_properties:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **recording_properties**

.. rst-class:: classref-property-setget

- void **set_recording_properties** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_recording_properties** **(** **)**

.. container:: contribute

	目前没有这个属性的描述。请帮我们\ :ref:`贡献一个 <doc_updating_the_class_reference>`\ ！

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
