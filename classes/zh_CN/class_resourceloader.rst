:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/ResourceLoader.xml.

.. _class_ResourceLoader:

ResourceLoader
==============

**继承：** :ref:`Object<class_Object>`

用于加载资源文件的单例。

.. rst-class:: classref-introduction-group

描述
----

用于从文件系统加载资源文件的单例。

会使用引擎中（内置或插件）注册的许多 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` 类将文件加载到内存中并将其转换为引擎可以使用的格式。

\ **注意：**\ 你需要先将文件导入引擎，才能使用 :ref:`load<class_ResourceLoader_method_load>` 进行加载。如果你想在运行时加载 :ref:`Image<class_Image>`\ ，可以使用 :ref:`Image.load<class_Image_method_load>`\ 。如果你想导入音频文件，可以使用 :ref:`AudioStreamMP3.data<class_AudioStreamMP3_property_data>` 中描述的代码段。

.. rst-class:: classref-introduction-group

教程
----

- `操作系统测试演示 <https://godotengine.org/asset-library/asset/677>`__

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                          | :ref:`add_resource_format_loader<class_ResourceLoader_method_add_resource_format_loader>` **(** :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` format_loader, :ref:`bool<class_bool>` at_front=false **)**                                                                 |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                                       | :ref:`exists<class_ResourceLoader_method_exists>` **(** :ref:`String<class_String>` path, :ref:`String<class_String>` type_hint="" **)**                                                                                                                                            |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>`             | :ref:`get_dependencies<class_ResourceLoader_method_get_dependencies>` **(** :ref:`String<class_String>` path **)**                                                                                                                                                                  |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>`             | :ref:`get_recognized_extensions_for_type<class_ResourceLoader_method_get_recognized_extensions_for_type>` **(** :ref:`String<class_String>` type **)**                                                                                                                              |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                                         | :ref:`get_resource_uid<class_ResourceLoader_method_get_resource_uid>` **(** :ref:`String<class_String>` path **)**                                                                                                                                                                  |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                                       | :ref:`has_cached<class_ResourceLoader_method_has_cached>` **(** :ref:`String<class_String>` path **)**                                                                                                                                                                              |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Resource<class_Resource>`                               | :ref:`load<class_ResourceLoader_method_load>` **(** :ref:`String<class_String>` path, :ref:`String<class_String>` type_hint="", :ref:`CacheMode<enum_ResourceLoader_CacheMode>` cache_mode=1 **)**                                                                                  |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Resource<class_Resource>`                               | :ref:`load_threaded_get<class_ResourceLoader_method_load_threaded_get>` **(** :ref:`String<class_String>` path **)**                                                                                                                                                                |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>` | :ref:`load_threaded_get_status<class_ResourceLoader_method_load_threaded_get_status>` **(** :ref:`String<class_String>` path, :ref:`Array<class_Array>` progress=[] **)**                                                                                                           |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>`                         | :ref:`load_threaded_request<class_ResourceLoader_method_load_threaded_request>` **(** :ref:`String<class_String>` path, :ref:`String<class_String>` type_hint="", :ref:`bool<class_bool>` use_sub_threads=false, :ref:`CacheMode<enum_ResourceLoader_CacheMode>` cache_mode=1 **)** |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                          | :ref:`remove_resource_format_loader<class_ResourceLoader_method_remove_resource_format_loader>` **(** :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` format_loader **)**                                                                                                   |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                          | :ref:`set_abort_on_missing_resources<class_ResourceLoader_method_set_abort_on_missing_resources>` **(** :ref:`bool<class_bool>` abort **)**                                                                                                                                         |
   +---------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

枚举
----

.. _enum_ResourceLoader_ThreadLoadStatus:

.. rst-class:: classref-enumeration

enum **ThreadLoadStatus**:

.. _class_ResourceLoader_constant_THREAD_LOAD_INVALID_RESOURCE:

.. rst-class:: classref-enumeration-constant

:ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>` **THREAD_LOAD_INVALID_RESOURCE** = ``0``

该资源无效，或尚未使用 :ref:`load_threaded_request<class_ResourceLoader_method_load_threaded_request>` 加载。

.. _class_ResourceLoader_constant_THREAD_LOAD_IN_PROGRESS:

.. rst-class:: classref-enumeration-constant

:ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>` **THREAD_LOAD_IN_PROGRESS** = ``1``

该资源仍在加载中。

.. _class_ResourceLoader_constant_THREAD_LOAD_FAILED:

.. rst-class:: classref-enumeration-constant

:ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>` **THREAD_LOAD_FAILED** = ``2``

加载过程中发生了错误，导致失败。

.. _class_ResourceLoader_constant_THREAD_LOAD_LOADED:

.. rst-class:: classref-enumeration-constant

:ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>` **THREAD_LOAD_LOADED** = ``3``

资源成功加载，可以通过 :ref:`load_threaded_get<class_ResourceLoader_method_load_threaded_get>` 访问。

.. rst-class:: classref-item-separator

----

.. _enum_ResourceLoader_CacheMode:

.. rst-class:: classref-enumeration

enum **CacheMode**:

.. _class_ResourceLoader_constant_CACHE_MODE_IGNORE:

.. rst-class:: classref-enumeration-constant

:ref:`CacheMode<enum_ResourceLoader_CacheMode>` **CACHE_MODE_IGNORE** = ``0``



.. _class_ResourceLoader_constant_CACHE_MODE_REUSE:

.. rst-class:: classref-enumeration-constant

:ref:`CacheMode<enum_ResourceLoader_CacheMode>` **CACHE_MODE_REUSE** = ``1``



.. _class_ResourceLoader_constant_CACHE_MODE_REPLACE:

.. rst-class:: classref-enumeration-constant

:ref:`CacheMode<enum_ResourceLoader_CacheMode>` **CACHE_MODE_REPLACE** = ``2``



.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_ResourceLoader_method_add_resource_format_loader:

.. rst-class:: classref-method

void **add_resource_format_loader** **(** :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` format_loader, :ref:`bool<class_bool>` at_front=false **)**

注册一个新的 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>`\ 。ResourceLoader 将会按照 :ref:`load<class_ResourceLoader_method_load>` 中的描述使用 ResourceFormatLoader。

对于用 GDScript 编写的 ResourceFormatLoader，此方法将隐式执行（详见 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>`\ ）。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_exists:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **exists** **(** :ref:`String<class_String>` path, :ref:`String<class_String>` type_hint="" **)**

返回给定路径 ``path`` 是否存在已识别的资源。

可选的 ``type_hint`` 可用于进一步指定 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` 应处理的 :ref:`Resource<class_Resource>` 类型。任何继承自 :ref:`Resource<class_Resource>` 的内容都可以用作类型提示，例如 :ref:`Image<class_Image>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_get_dependencies:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **get_dependencies** **(** :ref:`String<class_String>` path **)**

返回位于给定路径 ``path`` 的资源的依赖项。

\ **注意：**\ 返回的单个依赖项是由 ``::`` 分隔的切片。你可以使用 :ref:`String.get_slice<class_String_method_get_slice>` 来获取每段的内容。

::

    for dep in ResourceLoader.get_dependencies(path):
        print(dep.get_slice("::", 0)) # 输出 UID。
        print(dep.get_slice("::", 2)) # 输出路径。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_get_recognized_extensions_for_type:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **get_recognized_extensions_for_type** **(** :ref:`String<class_String>` type **)**

返回资源类型的已识别扩展名列表。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_get_resource_uid:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_resource_uid** **(** :ref:`String<class_String>` path **)**

返回与一个给定资源路径关联的 ID，如果不存在此类 ID，则返回 ``-1``\ 。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_has_cached:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has_cached** **(** :ref:`String<class_String>` path **)**

返回给定 ``path`` 的缓存资源是否可用。

一旦引擎加载了资源，它将被缓存在内存中以加快访问速度，未来调用 :ref:`load<class_ResourceLoader_method_load>` 方法将使用缓存版本。可以通过在具有相同路径的新资源上使用 :ref:`Resource.take_over_path<class_Resource_method_take_over_path>` 来覆盖缓存资源。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_load:

.. rst-class:: classref-method

:ref:`Resource<class_Resource>` **load** **(** :ref:`String<class_String>` path, :ref:`String<class_String>` type_hint="", :ref:`CacheMode<enum_ResourceLoader_CacheMode>` cache_mode=1 **)**

在给定的 ``path`` 中加载资源，并将结果缓存以供进一步访问。

按顺序查询注册的 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>`\ ，以找到可以处理文件扩展名的第一个 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>`\ ，然后尝试加载。如果加载失败，则还会尝试其余的 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>`\ 。

可选的 ``type_hint`` 可用于进一步指定 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` 应处理的 :ref:`Resource<class_Resource>` 类型。任何继承自 :ref:`Resource<class_Resource>` 的东西都可以用作类型提示，例如 :ref:`Image<class_Image>`\ 。

\ ``cache_mode`` 属性定义在加载资源时是否以及如何使用或更新缓存。详情见 :ref:`CacheMode<enum_ResourceLoader_CacheMode>`\ 。

如果没有 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` 可以处理该文件，则返回空资源。

GDScript 具有一个简化的 :ref:`@GDScript.load<class_@GDScript_method_load>` 内置方法，可在大多数情况下使用，而 **ResourceLoader** 供更高级的情况使用。

\ **注意：**\ 如果 :ref:`ProjectSettings.editor/export/convert_text_resources_to_binary<class_ProjectSettings_property_editor/export/convert_text_resources_to_binary>` 为 ``true``\ ，则 :ref:`@GDScript.load<class_@GDScript_method_load>` 无法在导出后的项目中读取已转换的文件。如果你需要在运行时加载存在于 PCK 中的文件，请将 :ref:`ProjectSettings.editor/export/convert_text_resources_to_binary<class_ProjectSettings_property_editor/export/convert_text_resources_to_binary>` 设置为 ``false``\ 。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_load_threaded_get:

.. rst-class:: classref-method

:ref:`Resource<class_Resource>` **load_threaded_get** **(** :ref:`String<class_String>` path **)**

返回由 :ref:`load_threaded_request<class_ResourceLoader_method_load_threaded_request>` 加载的资源。

如果在加载线程完成之前调用此方法（即 :ref:`load_threaded_get_status<class_ResourceLoader_method_load_threaded_get_status>` 不是 :ref:`THREAD_LOAD_LOADED<class_ResourceLoader_constant_THREAD_LOAD_LOADED>`\ ），则调用线程将被阻塞，直到资源加载完成。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_load_threaded_get_status:

.. rst-class:: classref-method

:ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>` **load_threaded_get_status** **(** :ref:`String<class_String>` path, :ref:`Array<class_Array>` progress=[] **)**

返回使用 :ref:`load_threaded_request<class_ResourceLoader_method_load_threaded_request>` 在 ``path`` 处启动的线程加载操作的状态。可能的返回值见 :ref:`ThreadLoadStatus<enum_ResourceLoader_ThreadLoadStatus>`\ 。

可以通过 ``progress`` 可选地传递一个数组变量，并返回一个包含线程加载完成百分比的单元素的数组。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_load_threaded_request:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **load_threaded_request** **(** :ref:`String<class_String>` path, :ref:`String<class_String>` type_hint="", :ref:`bool<class_bool>` use_sub_threads=false, :ref:`CacheMode<enum_ResourceLoader_CacheMode>` cache_mode=1 **)**

使用线程加载资源。如果 ``use_sub_threads`` 为 ``true``\ ，将使用多个线程来加载资源，这会使加载更快，但可能会影响主线程（从而导致游戏降速）。

\ ``cache_mode`` 属性定义在加载资源时是否以及如何使用或更新缓存。详情见 :ref:`CacheMode<enum_ResourceLoader_CacheMode>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_remove_resource_format_loader:

.. rst-class:: classref-method

void **remove_resource_format_loader** **(** :ref:`ResourceFormatLoader<class_ResourceFormatLoader>` format_loader **)**

取消注册给定的 :ref:`ResourceFormatLoader<class_ResourceFormatLoader>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_ResourceLoader_method_set_abort_on_missing_resources:

.. rst-class:: classref-method

void **set_abort_on_missing_resources** **(** :ref:`bool<class_bool>` abort **)**

更改缺少子资源时的行为。默认行为是中止加载。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
