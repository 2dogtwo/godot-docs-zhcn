:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/LightmapGIData.xml.

.. _class_LightmapGIData:

LightmapGIData
==============

**继承：** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

包含用于 :ref:`LightmapGI<class_LightmapGI>` 的烘焙光照贴图和动态对象探测数据。

.. rst-class:: classref-introduction-group

描述
----

**LightmapGIData** 包含用于 :ref:`LightmapGI<class_LightmapGI>` 的烘焙光照贴图和动态对象探测数据。在 :ref:`LightmapGI<class_LightmapGI>` 中每当光照贴图被烘焙时都会替换它。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-----------------------------------------------+---------------------------------------------------------------------------+--------+
   | :ref:`TextureLayered<class_TextureLayered>`   | :ref:`light_texture<class_LightmapGIData_property_light_texture>`         |        |
   +-----------------------------------------------+---------------------------------------------------------------------------+--------+
   | :ref:`TextureLayered[]<class_TextureLayered>` | :ref:`lightmap_textures<class_LightmapGIData_property_lightmap_textures>` | ``[]`` |
   +-----------------------------------------------+---------------------------------------------------------------------------+--------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                            | :ref:`add_user<class_LightmapGIData_method_add_user>` **(** :ref:`NodePath<class_NodePath>` path, :ref:`Rect2<class_Rect2>` uv_scale, :ref:`int<class_int>` slice_index, :ref:`int<class_int>` sub_instance **)** |
   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                            | :ref:`clear_users<class_LightmapGIData_method_clear_users>` **(** **)**                                                                                                                                           |
   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`           | :ref:`get_user_count<class_LightmapGIData_method_get_user_count>` **(** **)** |const|                                                                                                                             |
   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`NodePath<class_NodePath>` | :ref:`get_user_path<class_LightmapGIData_method_get_user_path>` **(** :ref:`int<class_int>` user_idx **)** |const|                                                                                                |
   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`         | :ref:`is_using_spherical_harmonics<class_LightmapGIData_method_is_using_spherical_harmonics>` **(** **)** |const|                                                                                                 |
   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                            | :ref:`set_uses_spherical_harmonics<class_LightmapGIData_method_set_uses_spherical_harmonics>` **(** :ref:`bool<class_bool>` uses_spherical_harmonics **)**                                                        |
   +---------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_LightmapGIData_property_light_texture:

.. rst-class:: classref-property

:ref:`TextureLayered<class_TextureLayered>` **light_texture**

.. rst-class:: classref-property-setget

- void **set_light_texture** **(** :ref:`TextureLayered<class_TextureLayered>` value **)**
- :ref:`TextureLayered<class_TextureLayered>` **get_light_texture** **(** **)**

由光照贴图器生成的光照贴图图集纹理。

\ *已弃用。*\ 光照贴图图集现在可以有多个纹理。请参阅 :ref:`lightmap_textures<class_LightmapGIData_property_lightmap_textures>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_LightmapGIData_property_lightmap_textures:

.. rst-class:: classref-property

:ref:`TextureLayered[]<class_TextureLayered>` **lightmap_textures** = ``[]``

.. rst-class:: classref-property-setget

- void **set_lightmap_textures** **(** :ref:`TextureLayered[]<class_TextureLayered>` value **)**
- :ref:`TextureLayered[]<class_TextureLayered>` **get_lightmap_textures** **(** **)**

由光照贴图器生成的光照贴图图集纹理。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_LightmapGIData_method_add_user:

.. rst-class:: classref-method

void **add_user** **(** :ref:`NodePath<class_NodePath>` path, :ref:`Rect2<class_Rect2>` uv_scale, :ref:`int<class_int>` slice_index, :ref:`int<class_int>` sub_instance **)**

添加一个在该 **LightmapGIData** 中被视为已烘焙的对象。

.. rst-class:: classref-item-separator

----

.. _class_LightmapGIData_method_clear_users:

.. rst-class:: classref-method

void **clear_users** **(** **)**

清除在该 **LightmapGIData** 中被视为已烘焙的所有对象。

.. rst-class:: classref-item-separator

----

.. _class_LightmapGIData_method_get_user_count:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_user_count** **(** **)** |const|

返回在该 **LightmapGIData** 中被视为烘焙的对象的数量。

.. rst-class:: classref-item-separator

----

.. _class_LightmapGIData_method_get_user_path:

.. rst-class:: classref-method

:ref:`NodePath<class_NodePath>` **get_user_path** **(** :ref:`int<class_int>` user_idx **)** |const|

返回索引 ``user_idx`` 处烘焙对象的 :ref:`NodePath<class_NodePath>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_LightmapGIData_method_is_using_spherical_harmonics:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_using_spherical_harmonics** **(** **)** |const|

如果为 ``true``\ ，则光照贴图使用定向信息烘焙。另请参阅 :ref:`LightmapGI.directional<class_LightmapGI_property_directional>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_LightmapGIData_method_set_uses_spherical_harmonics:

.. rst-class:: classref-method

void **set_uses_spherical_harmonics** **(** :ref:`bool<class_bool>` uses_spherical_harmonics **)**

如果 ``uses_spherical_harmonics`` 为 ``true``\ ，则告诉引擎将光照贴图数据视为使用了定向信息烘焙的。

\ **注意：**\ 在已烘焙的光照贴图上更改此值不会导致再次烘焙它们。这意味着在再次烘焙光照贴图之前，材质外观将看起来不正确，在这种情况下，此处设置的值将被丢弃，因为整个 **LightmapGIData** 资源被光照贴图器替换。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
