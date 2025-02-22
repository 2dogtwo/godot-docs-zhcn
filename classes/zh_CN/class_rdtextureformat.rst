:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/RDTextureFormat.xml.

.. _class_RDTextureFormat:

RDTextureFormat
===============

**继承：** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

纹理格式（由 :ref:`RenderingDevice<class_RenderingDevice>` 使用）。

.. rst-class:: classref-introduction-group

描述
----

这个对象由 :ref:`RenderingDevice<class_RenderingDevice>` 使用。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`int<class_int>`                                                        | :ref:`array_layers<class_RDTextureFormat_property_array_layers>` | ``1`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`int<class_int>`                                                        | :ref:`depth<class_RDTextureFormat_property_depth>`               | ``1`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`DataFormat<enum_RenderingDevice_DataFormat>`                           | :ref:`format<class_RDTextureFormat_property_format>`             | ``8`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`int<class_int>`                                                        | :ref:`height<class_RDTextureFormat_property_height>`             | ``1`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`int<class_int>`                                                        | :ref:`mipmaps<class_RDTextureFormat_property_mipmaps>`           | ``1`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`TextureSamples<enum_RenderingDevice_TextureSamples>`                   | :ref:`samples<class_RDTextureFormat_property_samples>`           | ``0`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`TextureType<enum_RenderingDevice_TextureType>`                         | :ref:`texture_type<class_RDTextureFormat_property_texture_type>` | ``1`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | |bitfield|\<:ref:`TextureUsageBits<enum_RenderingDevice_TextureUsageBits>`\> | :ref:`usage_bits<class_RDTextureFormat_property_usage_bits>`     | ``0`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+
   | :ref:`int<class_int>`                                                        | :ref:`width<class_RDTextureFormat_property_width>`               | ``1`` |
   +------------------------------------------------------------------------------+------------------------------------------------------------------+-------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +------+------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void | :ref:`add_shareable_format<class_RDTextureFormat_method_add_shareable_format>` **(** :ref:`DataFormat<enum_RenderingDevice_DataFormat>` format **)**       |
   +------+------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void | :ref:`remove_shareable_format<class_RDTextureFormat_method_remove_shareable_format>` **(** :ref:`DataFormat<enum_RenderingDevice_DataFormat>` format **)** |
   +------+------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_RDTextureFormat_property_array_layers:

.. rst-class:: classref-property

:ref:`int<class_int>` **array_layers** = ``1``

.. rst-class:: classref-property-setget

- void **set_array_layers** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_array_layers** **(** **)**

纹理的层数。仅适用于 2D 纹理数组。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_depth:

.. rst-class:: classref-property

:ref:`int<class_int>` **depth** = ``1``

.. rst-class:: classref-property-setget

- void **set_depth** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_depth** **(** **)**

纹理的深度（单位为像素）。2D 纹理始终为 ``1``\ 。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_format:

.. rst-class:: classref-property

:ref:`DataFormat<enum_RenderingDevice_DataFormat>` **format** = ``8``

.. rst-class:: classref-property-setget

- void **set_format** **(** :ref:`DataFormat<enum_RenderingDevice_DataFormat>` value **)**
- :ref:`DataFormat<enum_RenderingDevice_DataFormat>` **get_format** **(** **)**

纹理的像素数据格式。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_height:

.. rst-class:: classref-property

:ref:`int<class_int>` **height** = ``1``

.. rst-class:: classref-property-setget

- void **set_height** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_height** **(** **)**

纹理的高度（单位为像素）。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_mipmaps:

.. rst-class:: classref-property

:ref:`int<class_int>` **mipmaps** = ``1``

.. rst-class:: classref-property-setget

- void **set_mipmaps** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_mipmaps** **(** **)**

纹理中可用的 mipmap 数。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_samples:

.. rst-class:: classref-property

:ref:`TextureSamples<enum_RenderingDevice_TextureSamples>` **samples** = ``0``

.. rst-class:: classref-property-setget

- void **set_samples** **(** :ref:`TextureSamples<enum_RenderingDevice_TextureSamples>` value **)**
- :ref:`TextureSamples<enum_RenderingDevice_TextureSamples>` **get_samples** **(** **)**

对纹理进行采样时所使用的样本数。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_texture_type:

.. rst-class:: classref-property

:ref:`TextureType<enum_RenderingDevice_TextureType>` **texture_type** = ``1``

.. rst-class:: classref-property-setget

- void **set_texture_type** **(** :ref:`TextureType<enum_RenderingDevice_TextureType>` value **)**
- :ref:`TextureType<enum_RenderingDevice_TextureType>` **get_texture_type** **(** **)**

纹理类型。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_usage_bits:

.. rst-class:: classref-property

|bitfield|\<:ref:`TextureUsageBits<enum_RenderingDevice_TextureUsageBits>`\> **usage_bits** = ``0``

.. rst-class:: classref-property-setget

- void **set_usage_bits** **(** |bitfield|\<:ref:`TextureUsageBits<enum_RenderingDevice_TextureUsageBits>`\> value **)**
- |bitfield|\<:ref:`TextureUsageBits<enum_RenderingDevice_TextureUsageBits>`\> **get_usage_bits** **(** **)**

纹理的用途位，决定使用该纹理时能做什么。

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_property_width:

.. rst-class:: classref-property

:ref:`int<class_int>` **width** = ``1``

.. rst-class:: classref-property-setget

- void **set_width** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_width** **(** **)**

纹理的宽度（单位为像素）。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_RDTextureFormat_method_add_shareable_format:

.. rst-class:: classref-method

void **add_shareable_format** **(** :ref:`DataFormat<enum_RenderingDevice_DataFormat>` format **)**

.. container:: contribute

	目前没有这个方法的描述。请帮我们\ :ref:`贡献一个 <doc_updating_the_class_reference>`\ ！

.. rst-class:: classref-item-separator

----

.. _class_RDTextureFormat_method_remove_shareable_format:

.. rst-class:: classref-method

void **remove_shareable_format** **(** :ref:`DataFormat<enum_RenderingDevice_DataFormat>` format **)**

.. container:: contribute

	目前没有这个方法的描述。请帮我们\ :ref:`贡献一个 <doc_updating_the_class_reference>`\ ！

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
