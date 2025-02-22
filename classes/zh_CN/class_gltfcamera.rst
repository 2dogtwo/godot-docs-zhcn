:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/modules/gltf/doc_classes/GLTFCamera.xml.

.. _class_GLTFCamera:

GLTFCamera
==========

**继承：** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

代表 GLTF 相机。

.. rst-class:: classref-introduction-group

描述
----

代表基础 GLTF 规格中定义的相机。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`运行时文件加载与保存 <../tutorials/io/runtime_file_loading_and_saving>`

- `GLTF 相机的详细规格 <https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html#reference-camera>`__

- `GLTF 相机规格和示例文件 <https://github.com/KhronosGroup/glTF-Tutorials/blob/master/gltfTutorial/gltfTutorial_015_SimpleCameras.md>`__

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`depth_far<class_GLTFCamera_property_depth_far>`     | ``4000.0`` |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`depth_near<class_GLTFCamera_property_depth_near>`   | ``0.05``   |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`fov<class_GLTFCamera_property_fov>`                 | ``1.309``  |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`bool<class_bool>`   | :ref:`perspective<class_GLTFCamera_property_perspective>` | ``true``   |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`size_mag<class_GLTFCamera_property_size_mag>`       | ``0.5``    |
   +---------------------------+-----------------------------------------------------------+------------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`GLTFCamera<class_GLTFCamera>` | :ref:`from_dictionary<class_GLTFCamera_method_from_dictionary>` **(** :ref:`Dictionary<class_Dictionary>` dictionary **)** |static| |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`GLTFCamera<class_GLTFCamera>` | :ref:`from_node<class_GLTFCamera_method_from_node>` **(** :ref:`Camera3D<class_Camera3D>` camera_node **)** |static|                |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Dictionary<class_Dictionary>` | :ref:`to_dictionary<class_GLTFCamera_method_to_dictionary>` **(** **)** |const|                                                     |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Camera3D<class_Camera3D>`     | :ref:`to_node<class_GLTFCamera_method_to_node>` **(** **)** |const|                                                                 |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_GLTFCamera_property_depth_far:

.. rst-class:: classref-property

:ref:`float<class_float>` **depth_far** = ``4000.0``

.. rst-class:: classref-property-setget

- void **set_depth_far** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_depth_far** **(** **)**

该相机与远剔除边界的距离，相对于其本地 Z 轴，单位为米。映射到 GLTF 的 ``zfar`` 属性。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_depth_near:

.. rst-class:: classref-property

:ref:`float<class_float>` **depth_near** = ``0.05``

.. rst-class:: classref-property-setget

- void **set_depth_near** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_depth_near** **(** **)**

该相机与近剔除边界的距离，相对于其本地 Z 轴，单位为米。映射到 GLTF 的 ``znear`` 属性。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_fov:

.. rst-class:: classref-property

:ref:`float<class_float>` **fov** = ``1.309``

.. rst-class:: classref-property-setget

- void **set_fov** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_fov** **(** **)**

该相机的 FOV。这个类和 GLTF 在定义相机 FOV 时使用的都是弧度，但 Godot 使用的是度。映射到 GLTF 的 ``yfov`` 属性。只在透视相机中使用，即 :ref:`perspective<class_GLTFCamera_property_perspective>` 为 true 时。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_perspective:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **perspective** = ``true``

.. rst-class:: classref-property-setget

- void **set_perspective** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_perspective** **(** **)**

该相机是否处于透视模式。如果为 false，则该相机处于正交模式。映射到 GLTF 的相机 ``type`` 属性。详情见 :ref:`Camera3D.projection<class_Camera3D_property_projection>` 及 GLTF 规格。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_size_mag:

.. rst-class:: classref-property

:ref:`float<class_float>` **size_mag** = ``0.5``

.. rst-class:: classref-property-setget

- void **set_size_mag** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_size_mag** **(** **)**

该相机的大小。这个类和 GLTF 在定义相机大小尺度时使用的都是半径的米数，但 Godot 使用的是直径的米数。映射到 GLTF 的 ``ymag`` 属性。只在正交相机中使用，即 :ref:`perspective<class_GLTFCamera_property_perspective>` 为 false 时。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_GLTFCamera_method_from_dictionary:

.. rst-class:: classref-method

:ref:`GLTFCamera<class_GLTFCamera>` **from_dictionary** **(** :ref:`Dictionary<class_Dictionary>` dictionary **)** |static|

通过解析给定的 :ref:`Dictionary<class_Dictionary>` 新建 GLTFCamera 实例。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_method_from_node:

.. rst-class:: classref-method

:ref:`GLTFCamera<class_GLTFCamera>` **from_node** **(** :ref:`Camera3D<class_Camera3D>` camera_node **)** |static|

从给定的 Godot :ref:`Camera3D<class_Camera3D>` 节点新建 GLTFCamera 实例。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_method_to_dictionary:

.. rst-class:: classref-method

:ref:`Dictionary<class_Dictionary>` **to_dictionary** **(** **)** |const|

将这个 GLTFCamera 实例序列化为 :ref:`Dictionary<class_Dictionary>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_method_to_node:

.. rst-class:: classref-method

:ref:`Camera3D<class_Camera3D>` **to_node** **(** **)** |const|

将这个 GLTFCamera 实例转换为 Godot :ref:`Camera3D<class_Camera3D>` 节点。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
