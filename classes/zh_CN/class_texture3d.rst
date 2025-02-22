:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/Texture3D.xml.

.. _class_Texture3D:

Texture3D
=========

**继承：** :ref:`Texture<class_Texture>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

**派生：** :ref:`CompressedTexture3D<class_CompressedTexture3D>`, :ref:`ImageTexture3D<class_ImageTexture3D>`, :ref:`NoiseTexture3D<class_NoiseTexture3D>`, :ref:`PlaceholderTexture3D<class_PlaceholderTexture3D>`, :ref:`Texture3DRD<class_Texture3DRD>`

3D 纹理的基类。

.. rst-class:: classref-introduction-group

描述
----

:ref:`ImageTexture3D<class_ImageTexture3D>` 和 :ref:`CompressedTexture3D<class_CompressedTexture3D>` 的基类。无法直接使用，但包含所有访问派生资源类型所需的函数。\ **Texture3D** 是所有三维纹理类型的基类。另见 :ref:`TextureLayered<class_TextureLayered>`\ 。

所有图像都需要有相同的宽度、高度和 mipmap 层数。

要自己创建这样的纹理文件，请使用 Godot 编辑器的导入预设重新导入你的图像文件。

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`Image[]<class_Image>`      | :ref:`_get_data<class_Texture3D_private_method__get_data>` **(** **)** |virtual| |const|       |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`            | :ref:`_get_depth<class_Texture3D_private_method__get_depth>` **(** **)** |virtual| |const|     |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`Format<enum_Image_Format>` | :ref:`_get_format<class_Texture3D_private_method__get_format>` **(** **)** |virtual| |const|   |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`            | :ref:`_get_height<class_Texture3D_private_method__get_height>` **(** **)** |virtual| |const|   |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`            | :ref:`_get_width<class_Texture3D_private_method__get_width>` **(** **)** |virtual| |const|     |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`          | :ref:`_has_mipmaps<class_Texture3D_private_method__has_mipmaps>` **(** **)** |virtual| |const| |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`Resource<class_Resource>`  | :ref:`create_placeholder<class_Texture3D_method_create_placeholder>` **(** **)** |const|       |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`Image[]<class_Image>`      | :ref:`get_data<class_Texture3D_method_get_data>` **(** **)** |const|                           |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`            | :ref:`get_depth<class_Texture3D_method_get_depth>` **(** **)** |const|                         |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`Format<enum_Image_Format>` | :ref:`get_format<class_Texture3D_method_get_format>` **(** **)** |const|                       |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`            | :ref:`get_height<class_Texture3D_method_get_height>` **(** **)** |const|                       |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`            | :ref:`get_width<class_Texture3D_method_get_width>` **(** **)** |const|                         |
   +----------------------------------+------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`          | :ref:`has_mipmaps<class_Texture3D_method_has_mipmaps>` **(** **)** |const|                     |
   +----------------------------------+------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_Texture3D_private_method__get_data:

.. rst-class:: classref-method

:ref:`Image[]<class_Image>` **_get_data** **(** **)** |virtual| |const|

查询该 **Texture3D** 的数据时被调用。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_private_method__get_depth:

.. rst-class:: classref-method

:ref:`int<class_int>` **_get_depth** **(** **)** |virtual| |const|

查询该 **Texture3D** 的深度时被调用。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_private_method__get_format:

.. rst-class:: classref-method

:ref:`Format<enum_Image_Format>` **_get_format** **(** **)** |virtual| |const|

查询该 **Texture3D** 的格式时被调用。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_private_method__get_height:

.. rst-class:: classref-method

:ref:`int<class_int>` **_get_height** **(** **)** |virtual| |const|

查询该 **Texture3D** 的高度时被调用。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_private_method__get_width:

.. rst-class:: classref-method

:ref:`int<class_int>` **_get_width** **(** **)** |virtual| |const|

查询该 **Texture3D** 的宽度时被调用。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_private_method__has_mipmaps:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **_has_mipmaps** **(** **)** |virtual| |const|

查询该 **Texture3D** 的 Mipmap 是否存在时被调用。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_create_placeholder:

.. rst-class:: classref-method

:ref:`Resource<class_Resource>` **create_placeholder** **(** **)** |const|

创建该资源的占位符版本（\ :ref:`PlaceholderTexture3D<class_PlaceholderTexture3D>`\ ）。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_get_data:

.. rst-class:: classref-method

:ref:`Image[]<class_Image>` **get_data** **(** **)** |const|

将该 **Texture3D** 的数据作为 :ref:`Image<class_Image>` 数组返回。每个 :ref:`Image<class_Image>` 代表该 **Texture3D** 的一个\ *切片*\ ，不同的切片映射到不同的深度（Z 轴）级别。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_get_depth:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_depth** **(** **)** |const|

返回该 **Texture3D** 的深度，单位为像素。深度通常由 Z 轴表示（\ :ref:`Texture2D<class_Texture2D>` 中没有这个维度）。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_get_format:

.. rst-class:: classref-method

:ref:`Format<enum_Image_Format>` **get_format** **(** **)** |const|

返回纹理当前使用的格式。详情见 :ref:`Format<enum_Image_Format>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_get_height:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_height** **(** **)** |const|

返回该 **Texture3D** 的高度，单位为像素。宽度通常由 Y 轴表示。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_get_width:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_width** **(** **)** |const|

返回该 **Texture3D** 的宽度，单位为像素。宽度通常由 X 轴表示。

.. rst-class:: classref-item-separator

----

.. _class_Texture3D_method_has_mipmaps:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has_mipmaps** **(** **)** |const|

如果该 **Texture3D** 已生成 mipmap，则返回 ``true``\ 。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
