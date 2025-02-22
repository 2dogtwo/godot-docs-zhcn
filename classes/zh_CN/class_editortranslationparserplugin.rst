:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/EditorTranslationParserPlugin.xml.

.. _class_EditorTranslationParserPlugin:

EditorTranslationParserPlugin
=============================

**继承：** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

用于添加自定义解析器，以从自定义文件（.csv、.json等）提取已翻译的字符串的插件。

.. rst-class:: classref-introduction-group

描述
----

**EditorTranslationParserPlugin**\ 在文件被解析以提取需要翻译的字符串时被调用。为了定义解析和提取字符串的逻辑，在脚本中覆盖 :ref:`_parse_file<class_EditorTranslationParserPlugin_private_method__parse_file>` 方法。

如果使用上下文或复数形式，则将提取的字符串添加到参数 ``msgids`` 或 ``msgids_context_plural``\ 。

添加到 ``msgids_context_plural`` 时，必须使用格式 ``["A", "B", "C"]`` 添加数据，其中 ``A`` 表示提取的字符串，\ ``B`` 表示上下文，\ ``C`` 表示提取的字符串的复数形式。如果只想添加上下文而不添加复数形式，请将 ``""`` 用于复数形式槽。如果只想添加复数形式而不是上下文，做法也是一样的。有关具体示例，请参阅下面的代码。

提取的字符串将被写入用户在“项目设置”菜单的“本地化”选项卡中的“POT 生成”下选择的 POT 文件中。

下面显示了一个自定义解析器的示例，该解析器从 CSV 文件中提取字符串以写入 POT 中。


.. tabs::

 .. code-tab:: gdscript

    @tool
    extends EditorTranslationParserPlugin
    
    func _parse_file(path, msgids, msgids_context_plural):
        var file = FileAccess.open(path, FileAccess.READ)
        var text = file.get_as_text()
        var split_strs = text.split(",", false)
        for s in split_strs:
            msgids.append(s)
            #print("提取的字符串：" + s)
    
    func _get_recognized_extensions():
        return ["csv"]

 .. code-tab:: csharp

    using Godot;
    
    [Tool]
    public partial class CustomParser : EditorTranslationParserPlugin
    {
        public override void _ParseFile(string path, Godot.Collections.Array<string> msgids, Godot.Collections.Array<Godot.Collections.Array> msgidsContextPlural)
        {
            using var file = FileAccess.Open(path, FileAccess.ModeFlags.Read);
            string text = file.GetAsText();
            string[] splitStrs = text.Split(",", allowEmpty: false);
            foreach (string s in splitStrs)
            {
                msgids.Add(s);
                //GD.Print($"提取的字符串：{s}");
            }
        }
    
        public override string[] _GetRecognizedExtensions()
        {
            return new string[] { "csv" };
        }
    }



要添加一个与上下文或复数关联的可翻译字符串，请将其添加到 ``msgids_context_plural``\ ：


.. tabs::

 .. code-tab:: gdscript

    # 这将添加一条消息，其中 msgid 为“测试 1”、msgctxt 为“上下文”，以及 msgid_plural 为“测试 1 复数形式”。
    msgids_context_plural.append(["测试 1", "上下文", "测试 1 复数形式"])
    # 这将添加一条消息，其中 msgid 为“一个没有上下文的测试”、msgid_plural 为 “复数形式”。
    msgids_context_plural.append(["一个没有上下文的测试", "", "复数形式"])
    # 这将添加一条消息，其中 msgid 为“仅带有上下文”、msgctxt 为 “一条友好的上下文”。
    msgids_context_plural.append(["仅带有上下文", "一条友好的上下文", ""])

 .. code-tab:: csharp

    // 这将添加一条消息，其中 msgid 为“测试 1”、msgctxt 为“上下文”，以及 msgid_plural 为“测试 1 复数形式”。
    msgidsContextPlural.Add(new Godot.Collections.Array{"测试 1", "上下文", "测试 1 复数形式"});
    // 这将添加一条消息，其中 msgid 为“一个没有上下文的测试”、msgid_plural 为 “复数形式”。
    msgidsContextPlural.Add(new Godot.Collections.Array{"一个没有上下文的测试", "", "复数形式"});
    // 这将添加一条消息，其中 msgid 为“仅带有上下文”、msgctxt 为 “一条友好的上下文”。
    msgidsContextPlural.Add(new Godot.Collections.Array{"仅带有上下文", "一条友好的上下文", ""});



\ **注意：**\ 如果覆盖了标准脚本类型（GDScript、C# 等）的解析逻辑，最好使用 :ref:`ResourceLoader.load<class_ResourceLoader_method_load>` 加载 ``path`` 参数。这是因为内置脚本被加载为 :ref:`Resource<class_Resource>` 类型，而不是 :ref:`FileAccess<class_FileAccess>` 类型。

例如：


.. tabs::

 .. code-tab:: gdscript

    func _parse_file(path, msgids, msgids_context_plural):
        var res = ResourceLoader.load(path, "Script")
        var text = res.source_code
        # 解析逻辑。
    
    func _get_recognized_extensions():
        return ["gd"]

 .. code-tab:: csharp

    public override void _ParseFile(string path, Godot.Collections.Array<string> msgids, Godot.Collections.Array<Godot.Collections.Array> msgidsContextPlural)
    {
        var res = ResourceLoader.Load<Script>(path, "Script");
        string text = res.SourceCode;
        // 解析逻辑。
    }
    
    public override string[] _GetRecognizedExtensions()
    {
        return new string[] { "gd" };
    }



要使用 **EditorTranslationParserPlugin**\ ，请先使用 :ref:`EditorPlugin.add_translation_parser_plugin<class_EditorPlugin_method_add_translation_parser_plugin>` 方法注册它。

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>` | :ref:`_get_recognized_extensions<class_EditorTranslationParserPlugin_private_method__get_recognized_extensions>` **(** **)** |virtual| |const|                                                                                     |
   +---------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`_parse_file<class_EditorTranslationParserPlugin_private_method__parse_file>` **(** :ref:`String<class_String>` path, :ref:`String[]<class_String>` msgids, :ref:`Array[]<class_Array>` msgids_context_plural **)** |virtual| |
   +---------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_EditorTranslationParserPlugin_private_method__get_recognized_extensions:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **_get_recognized_extensions** **(** **)** |virtual| |const|

获取与该解析器关联的文件扩展名列表，例如 ``["csv"]``\ 。

.. rst-class:: classref-item-separator

----

.. _class_EditorTranslationParserPlugin_private_method__parse_file:

.. rst-class:: classref-method

void **_parse_file** **(** :ref:`String<class_String>` path, :ref:`String[]<class_String>` msgids, :ref:`Array[]<class_Array>` msgids_context_plural **)** |virtual|

覆盖该方法，定义自定义解析逻辑以提取可翻译的字符串。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
