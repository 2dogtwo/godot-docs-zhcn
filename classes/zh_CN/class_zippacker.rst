:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/modules/zip/doc_classes/ZIPPacker.xml.

.. _class_ZIPPacker:

ZIPPacker
=========

**继承：** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

允许创建 zip 文件。

.. rst-class:: classref-introduction-group

描述
----

该类实现了一个写入器，可以将多个 blob 存储在一个压缩文件中。

::

    func write_zip_file():
        var writer := ZIPPacker.new()
        var err := writer.open("user://archive.zip")
        if err != OK:
            return err
        writer.start_file("hello.txt")
        writer.write_file("Hello World".to_utf8_buffer())
        writer.close_file()
    
        writer.close()
        return OK

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>` | :ref:`close<class_ZIPPacker_method_close>` **(** **)**                                                                                     |
   +---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>` | :ref:`close_file<class_ZIPPacker_method_close_file>` **(** **)**                                                                           |
   +---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>` | :ref:`open<class_ZIPPacker_method_open>` **(** :ref:`String<class_String>` path, :ref:`ZipAppend<enum_ZIPPacker_ZipAppend>` append=0 **)** |
   +---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>` | :ref:`start_file<class_ZIPPacker_method_start_file>` **(** :ref:`String<class_String>` path **)**                                          |
   +---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>` | :ref:`write_file<class_ZIPPacker_method_write_file>` **(** :ref:`PackedByteArray<class_PackedByteArray>` data **)**                        |
   +---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

枚举
----

.. _enum_ZIPPacker_ZipAppend:

.. rst-class:: classref-enumeration

enum **ZipAppend**:

.. _class_ZIPPacker_constant_APPEND_CREATE:

.. rst-class:: classref-enumeration-constant

:ref:`ZipAppend<enum_ZIPPacker_ZipAppend>` **APPEND_CREATE** = ``0``

在给定的路径新建 Zip 归档文件。

.. _class_ZIPPacker_constant_APPEND_CREATEAFTER:

.. rst-class:: classref-enumeration-constant

:ref:`ZipAppend<enum_ZIPPacker_ZipAppend>` **APPEND_CREATEAFTER** = ``1``

在位于给定路径的已有文件的末尾追加新的 Zip 归档文件。

.. _class_ZIPPacker_constant_APPEND_ADDINZIP:

.. rst-class:: classref-enumeration-constant

:ref:`ZipAppend<enum_ZIPPacker_ZipAppend>` **APPEND_ADDINZIP** = ``2``

在位于给定路径的已有 Zip 归档文件中添加新文件。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_ZIPPacker_method_close:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **close** **(** **)**

关闭该实例底层所使用的资源。

.. rst-class:: classref-item-separator

----

.. _class_ZIPPacker_method_close_file:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **close_file** **(** **)**

停止向归档中的文件进行写入。

如果没有打开文件，则会失败。

.. rst-class:: classref-item-separator

----

.. _class_ZIPPacker_method_open:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **open** **(** :ref:`String<class_String>` path, :ref:`ZipAppend<enum_ZIPPacker_ZipAppend>` append=0 **)**

打开给定路径处的 Zip 文件，使用指定的写入模式进行写入。

必须在其他调用前调用。

.. rst-class:: classref-item-separator

----

.. _class_ZIPPacker_method_start_file:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **start_file** **(** :ref:`String<class_String>` path **)**

开始向存档中的一个文件写入。同一时间只能写一个文件。

必须在\ :ref:`open<class_ZIPPacker_method_open>`\ 之后调用。

.. rst-class:: classref-item-separator

----

.. _class_ZIPPacker_method_write_file:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **write_file** **(** :ref:`PackedByteArray<class_PackedByteArray>` data **)**

将给定的 ``data`` 写到文件中。

需要在 :ref:`start_file<class_ZIPPacker_method_start_file>` 之后调用。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
