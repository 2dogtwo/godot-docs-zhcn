:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/AnimationPlayer.xml.

.. _class_AnimationPlayer:

AnimationPlayer
===============

**继承：** :ref:`AnimationMixer<class_AnimationMixer>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

用于播放动画的节点。

.. rst-class:: classref-introduction-group

描述
----

动画播放器用于动画的通用播放。它包含 :ref:`AnimationLibrary<class_AnimationLibrary>` 资源的字典和动画过渡之间的自定义混合时间。

某些方法和属性使用单个键直接引用动画。这些键的格式为动画库的键，后跟正斜杠，然后是动画库内动画的键，例如 ``"movement/run"``\ 。如果动画库的键为空字符串（称为默认库），则省略正斜杠，与动画库使用相同的键。

\ **AnimationPlayer** 比 :ref:`Tween<class_Tween>` 更适合用于复杂动画，例如不规则计时的动画。如果用动画轨道编辑器比用代码实现更方便，也可以优先于 :ref:`Tween<class_Tween>` 使用。

更新动画的目标属性是在处理帧中进行的。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`2D 精灵动画 <../tutorials/2d/2d_sprite_animation>`

- :doc:`动画教程索引 <../tutorials/animation/index>`

- `第三人称射击演示 <https://godotengine.org/asset-library/asset/678>`__

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`String<class_String>` | :ref:`assigned_animation<class_AnimationPlayer_property_assigned_animation>`                   |           |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`String<class_String>` | :ref:`autoplay<class_AnimationPlayer_property_autoplay>`                                       | ``""``    |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`String<class_String>` | :ref:`current_animation<class_AnimationPlayer_property_current_animation>`                     | ``""``    |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`   | :ref:`current_animation_length<class_AnimationPlayer_property_current_animation_length>`       |           |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`   | :ref:`current_animation_position<class_AnimationPlayer_property_current_animation_position>`   |           |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`bool<class_bool>`     | :ref:`movie_quit_on_finish<class_AnimationPlayer_property_movie_quit_on_finish>`               | ``false`` |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`   | :ref:`playback_default_blend_time<class_AnimationPlayer_property_playback_default_blend_time>` | ``0.0``   |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+
   | :ref:`float<class_float>`   | :ref:`speed_scale<class_AnimationPlayer_property_speed_scale>`                                 | ``1.0``   |
   +-----------------------------+------------------------------------------------------------------------------------------------+-----------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`StringName<class_StringName>`                                            | :ref:`animation_get_next<class_AnimationPlayer_method_animation_get_next>` **(** :ref:`StringName<class_StringName>` animation_from **)** |const|                                                                                     |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`animation_set_next<class_AnimationPlayer_method_animation_set_next>` **(** :ref:`StringName<class_StringName>` animation_from, :ref:`StringName<class_StringName>` animation_to **)**                                           |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`clear_queue<class_AnimationPlayer_method_clear_queue>` **(** **)**                                                                                                                                                              |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                                                      | :ref:`get_blend_time<class_AnimationPlayer_method_get_blend_time>` **(** :ref:`StringName<class_StringName>` animation_from, :ref:`StringName<class_StringName>` animation_to **)** |const|                                           |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`AnimationMethodCallMode<enum_AnimationPlayer_AnimationMethodCallMode>`   | :ref:`get_method_call_mode<class_AnimationPlayer_method_get_method_call_mode>` **(** **)** |const|                                                                                                                                    |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                                                      | :ref:`get_playing_speed<class_AnimationPlayer_method_get_playing_speed>` **(** **)** |const|                                                                                                                                          |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` | :ref:`get_process_callback<class_AnimationPlayer_method_get_process_callback>` **(** **)** |const|                                                                                                                                    |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>`                              | :ref:`get_queue<class_AnimationPlayer_method_get_queue>` **(** **)**                                                                                                                                                                  |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`NodePath<class_NodePath>`                                                | :ref:`get_root<class_AnimationPlayer_method_get_root>` **(** **)** |const|                                                                                                                                                            |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                                                        | :ref:`is_playing<class_AnimationPlayer_method_is_playing>` **(** **)** |const|                                                                                                                                                        |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`pause<class_AnimationPlayer_method_pause>` **(** **)**                                                                                                                                                                          |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`play<class_AnimationPlayer_method_play>` **(** :ref:`StringName<class_StringName>` name="", :ref:`float<class_float>` custom_blend=-1, :ref:`float<class_float>` custom_speed=1.0, :ref:`bool<class_bool>` from_end=false **)** |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`play_backwards<class_AnimationPlayer_method_play_backwards>` **(** :ref:`StringName<class_StringName>` name="", :ref:`float<class_float>` custom_blend=-1 **)**                                                                 |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`queue<class_AnimationPlayer_method_queue>` **(** :ref:`StringName<class_StringName>` name **)**                                                                                                                                 |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`seek<class_AnimationPlayer_method_seek>` **(** :ref:`float<class_float>` seconds, :ref:`bool<class_bool>` update=false, :ref:`bool<class_bool>` update_only=false **)**                                                         |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`set_blend_time<class_AnimationPlayer_method_set_blend_time>` **(** :ref:`StringName<class_StringName>` animation_from, :ref:`StringName<class_StringName>` animation_to, :ref:`float<class_float>` sec **)**                    |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`set_method_call_mode<class_AnimationPlayer_method_set_method_call_mode>` **(** :ref:`AnimationMethodCallMode<enum_AnimationPlayer_AnimationMethodCallMode>` mode **)**                                                          |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`set_process_callback<class_AnimationPlayer_method_set_process_callback>` **(** :ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` mode **)**                                                        |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`set_root<class_AnimationPlayer_method_set_root>` **(** :ref:`NodePath<class_NodePath>` path **)**                                                                                                                               |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                                           | :ref:`stop<class_AnimationPlayer_method_stop>` **(** :ref:`bool<class_bool>` keep_state=false **)**                                                                                                                                   |
   +--------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

信号
----

.. _class_AnimationPlayer_signal_animation_changed:

.. rst-class:: classref-signal

**animation_changed** **(** :ref:`StringName<class_StringName>` old_name, :ref:`StringName<class_StringName>` new_name **)**

在前一个动画完成后，队列中的动画播放时发出。另见 :ref:`queue<class_AnimationPlayer_method_queue>`\ 。

\ **注意：**\ 通过 :ref:`play<class_AnimationPlayer_method_play>` 或 :ref:`AnimationTree<class_AnimationTree>` 改变动画时，不会发出此信号。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_signal_current_animation_changed:

.. rst-class:: classref-signal

**current_animation_changed** **(** :ref:`String<class_String>` name **)**

当 :ref:`current_animation<class_AnimationPlayer_property_current_animation>` 更改时发出。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

枚举
----

.. _enum_AnimationPlayer_AnimationProcessCallback:

.. rst-class:: classref-enumeration

enum **AnimationProcessCallback**:

.. _class_AnimationPlayer_constant_ANIMATION_PROCESS_PHYSICS:

.. rst-class:: classref-enumeration-constant

:ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` **ANIMATION_PROCESS_PHYSICS** = ``0``

用于向后兼容。见 :ref:`AnimationMixer.ANIMATION_CALLBACK_MODE_PROCESS_PHYSICS<class_AnimationMixer_constant_ANIMATION_CALLBACK_MODE_PROCESS_PHYSICS>`\ 。

.. _class_AnimationPlayer_constant_ANIMATION_PROCESS_IDLE:

.. rst-class:: classref-enumeration-constant

:ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` **ANIMATION_PROCESS_IDLE** = ``1``

用于向后兼容。见 :ref:`AnimationMixer.ANIMATION_CALLBACK_MODE_PROCESS_IDLE<class_AnimationMixer_constant_ANIMATION_CALLBACK_MODE_PROCESS_IDLE>`\ 。

.. _class_AnimationPlayer_constant_ANIMATION_PROCESS_MANUAL:

.. rst-class:: classref-enumeration-constant

:ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` **ANIMATION_PROCESS_MANUAL** = ``2``

用于向后兼容。见 :ref:`AnimationMixer.ANIMATION_CALLBACK_MODE_PROCESS_MANUAL<class_AnimationMixer_constant_ANIMATION_CALLBACK_MODE_PROCESS_MANUAL>`\ 。

.. rst-class:: classref-item-separator

----

.. _enum_AnimationPlayer_AnimationMethodCallMode:

.. rst-class:: classref-enumeration

enum **AnimationMethodCallMode**:

.. _class_AnimationPlayer_constant_ANIMATION_METHOD_CALL_DEFERRED:

.. rst-class:: classref-enumeration-constant

:ref:`AnimationMethodCallMode<enum_AnimationPlayer_AnimationMethodCallMode>` **ANIMATION_METHOD_CALL_DEFERRED** = ``0``

用于向后兼容。见 :ref:`AnimationMixer.ANIMATION_CALLBACK_MODE_METHOD_DEFERRED<class_AnimationMixer_constant_ANIMATION_CALLBACK_MODE_METHOD_DEFERRED>`\ 。

.. _class_AnimationPlayer_constant_ANIMATION_METHOD_CALL_IMMEDIATE:

.. rst-class:: classref-enumeration-constant

:ref:`AnimationMethodCallMode<enum_AnimationPlayer_AnimationMethodCallMode>` **ANIMATION_METHOD_CALL_IMMEDIATE** = ``1``

用于向后兼容。见 :ref:`AnimationMixer.ANIMATION_CALLBACK_MODE_METHOD_IMMEDIATE<class_AnimationMixer_constant_ANIMATION_CALLBACK_MODE_METHOD_IMMEDIATE>`\ 。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_AnimationPlayer_property_assigned_animation:

.. rst-class:: classref-property

:ref:`String<class_String>` **assigned_animation**

.. rst-class:: classref-property-setget

- void **set_assigned_animation** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_assigned_animation** **(** **)**

如果正在播放，则为当前动画的键，否则为上次播放的动画。设置后会改变动画，但除非已经播放，否则不会播放。另见 :ref:`current_animation<class_AnimationPlayer_property_current_animation>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_autoplay:

.. rst-class:: classref-property

:ref:`String<class_String>` **autoplay** = ``""``

.. rst-class:: classref-property-setget

- void **set_autoplay** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_autoplay** **(** **)**

场景加载时要播放的动画名称。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_current_animation:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_animation** = ``""``

.. rst-class:: classref-property-setget

- void **set_current_animation** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_current_animation** **(** **)**

当前播放的动画的名称。如果没有动画正在播放，该属性的值是一个空字符串。改变这个值不会重新启动动画。关于播放动画的更多信息请参阅 :ref:`play<class_AnimationPlayer_method_play>`\ 。

\ **注意：**\ 虽然这个属性会出现在检查器中，但它不是用来编辑的，也不会保存在场景中。该属性主要用于获取当前播放的动画，内部用于动画播放轨道。详情请参阅 :ref:`Animation<class_Animation>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_current_animation_length:

.. rst-class:: classref-property

:ref:`float<class_float>` **current_animation_length**

.. rst-class:: classref-property-setget

- :ref:`float<class_float>` **get_current_animation_length** **(** **)**

当前正在播放的动画的长度（以秒为单位）。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_current_animation_position:

.. rst-class:: classref-property

:ref:`float<class_float>` **current_animation_position**

.. rst-class:: classref-property-setget

- :ref:`float<class_float>` **get_current_animation_position** **(** **)**

当前播放的动画的位置（以秒为单位）。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_movie_quit_on_finish:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **movie_quit_on_finish** = ``false``

.. rst-class:: classref-property-setget

- void **set_movie_quit_on_finish_enabled** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_movie_quit_on_finish_enabled** **(** **)**

如果为 ``true``\ ，并且引擎在 Movie Maker 模式下运行（见 :ref:`MovieWriter<class_MovieWriter>`\ ），则会在此 **AnimationPlayer** 中播放完动画后，立即使用 :ref:`SceneTree.quit<class_SceneTree_method_quit>` 退出引擎。当引擎因此而退出时，会打印一条消息。

\ **注意：**\ 这与 :ref:`AnimationMixer.animation_finished<class_AnimationMixer_signal_animation_finished>` 信号遵循相同的逻辑，因此如果动画被设置为循环，它不会退出引擎。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_playback_default_blend_time:

.. rst-class:: classref-property

:ref:`float<class_float>` **playback_default_blend_time** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_default_blend_time** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_default_blend_time** **(** **)**

混合动画的默认时间。范围从 0 到 4096，精度为 0.01。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_property_speed_scale:

.. rst-class:: classref-property

:ref:`float<class_float>` **speed_scale** = ``1.0``

.. rst-class:: classref-property-setget

- void **set_speed_scale** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_speed_scale** **(** **)**

速度缩放比。例如，如果该值为 ``1``\ ，则动画以正常速度播放。如果它是 ``0.5``\ ，那么它会半速播放。如果是 ``2``\ ，则会以双倍速度播放。

如果设置为负值，则动画反向播放。如果设置为\ ``0``\ ，则动画不会前进。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_AnimationPlayer_method_animation_get_next:

.. rst-class:: classref-method

:ref:`StringName<class_StringName>` **animation_get_next** **(** :ref:`StringName<class_StringName>` animation_from **)** |const|

返回在 ``animation_from`` 动画之后排队播放的动画的键。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_animation_set_next:

.. rst-class:: classref-method

void **animation_set_next** **(** :ref:`StringName<class_StringName>` animation_from, :ref:`StringName<class_StringName>` animation_to **)**

当 ``animation_from`` 动画完成时，触发 ``animation_to`` 动画。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_clear_queue:

.. rst-class:: classref-method

void **clear_queue** **(** **)**

清除所有已排队、未播放的动画。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_get_blend_time:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_blend_time** **(** :ref:`StringName<class_StringName>` animation_from, :ref:`StringName<class_StringName>` animation_to **)** |const|

返回两个动画之间的混合时间（以秒为单位），由它们的键引用。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_get_method_call_mode:

.. rst-class:: classref-method

:ref:`AnimationMethodCallMode<enum_AnimationPlayer_AnimationMethodCallMode>` **get_method_call_mode** **(** **)** |const|

用于向后兼容。见 :ref:`AnimationCallbackModeMethod<enum_AnimationMixer_AnimationCallbackModeMethod>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_get_playing_speed:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_playing_speed** **(** **)** |const|

返回当前动画的实际播放速度，未播放时则为 ``0``\ 。这个速度是 :ref:`speed_scale<class_AnimationPlayer_property_speed_scale>` 属性乘以调用 :ref:`play<class_AnimationPlayer_method_play>` 时指定的 ``custom_speed`` 参数。

如果当前动画是倒放的，则返回负值。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_get_process_callback:

.. rst-class:: classref-method

:ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` **get_process_callback** **(** **)** |const|

用于向后兼容。见 :ref:`AnimationCallbackModeProcess<enum_AnimationMixer_AnimationCallbackModeProcess>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_get_queue:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **get_queue** **(** **)**

返回当前排队播放的动画键列表。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_get_root:

.. rst-class:: classref-method

:ref:`NodePath<class_NodePath>` **get_root** **(** **)** |const|

用于向后兼容。见 :ref:`AnimationMixer.root_node<class_AnimationMixer_property_root_node>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_is_playing:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_playing** **(** **)** |const|

如果动画目前正在播放，则返回 ``true``\ （即便 :ref:`speed_scale<class_AnimationPlayer_property_speed_scale>` 和/或 ``custom_speed`` 为 ``0``\ ）。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_pause:

.. rst-class:: classref-method

void **pause** **(** **)**

暂停当前播放的动画。\ :ref:`current_animation_position<class_AnimationPlayer_property_current_animation_position>` 将被保留，调用 :ref:`play<class_AnimationPlayer_method_play>` 或 :ref:`play_backwards<class_AnimationPlayer_method_play_backwards>` 时，不带参数或使用与 :ref:`assigned_animation<class_AnimationPlayer_property_assigned_animation>` 相同的动画名称，将恢复动画。

另见 :ref:`stop<class_AnimationPlayer_method_stop>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_play:

.. rst-class:: classref-method

void **play** **(** :ref:`StringName<class_StringName>` name="", :ref:`float<class_float>` custom_blend=-1, :ref:`float<class_float>` custom_speed=1.0, :ref:`bool<class_bool>` from_end=false **)**

播放键名为 ``name`` 的动画。可以设置自定义混合时间和速度。

\ ``from_end`` 选项仅在切换到新的动画轨道，或在相同轨道的开始或结束时生效。它不影响在动画被中途暂停时恢复播放。如果 ``custom_speed`` 为负，且 ``from_end`` 为 ``true``\ ，则动画将向后播放（相当于调用 :ref:`play_backwards<class_AnimationPlayer_method_play_backwards>`\ ）。

\ **AnimationPlayer** 使用 :ref:`assigned_animation<class_AnimationPlayer_property_assigned_animation>` 跟踪其当前或上次播放的动画。如果使用相同的动画 ``name`` 或没有 ``name`` 参数调用此方法，则分配的动画将在暂停时恢复播放。

\ **注意：**\ 动画将在下次处理 **AnimationPlayer** 时更新。如果在调用该方法的同时更新了其他变量，则它们可能更新得太早。要立即执行更新，请调用 ``advance(0)``\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_play_backwards:

.. rst-class:: classref-method

void **play_backwards** **(** :ref:`StringName<class_StringName>` name="", :ref:`float<class_float>` custom_blend=-1 **)**

倒放名称键为 ``name`` 的动画。

这个方法是简写，等价于调用 :ref:`play<class_AnimationPlayer_method_play>` 时使用 ``custom_speed = -1.0`` 和 ``from_end = true``\ ，所以更多信息请参阅其描述。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_queue:

.. rst-class:: classref-method

void **queue** **(** :ref:`StringName<class_StringName>` name **)**

将动画加入队列，在当前动画播放完毕后播放。

\ **注意：**\ 如果当前正在播放循环动画，除非以某种方式停止循环动画，否则排队的动画将永远不会播放。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_seek:

.. rst-class:: classref-method

void **seek** **(** :ref:`float<class_float>` seconds, :ref:`bool<class_bool>` update=false, :ref:`bool<class_bool>` update_only=false **)**

将动画寻道到时间点 ``seconds``\ （单位为秒）。\ ``update`` 为 ``true`` 时会同时更新动画，否则会在处理时更新。当前帧和 ``seconds`` 之间的事件会被跳过。

如果 ``update_only`` 为 true，则不会处理方法轨道、音频轨道、动画播放轨道。

\ **注意：**\ 寻道至动画的末尾不会触发 :ref:`AnimationMixer.animation_finished<class_AnimationMixer_signal_animation_finished>`\ 。如果想要跳过动画并触发该信号，请使用 :ref:`AnimationMixer.advance<class_AnimationMixer_method_advance>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_set_blend_time:

.. rst-class:: classref-method

void **set_blend_time** **(** :ref:`StringName<class_StringName>` animation_from, :ref:`StringName<class_StringName>` animation_to, :ref:`float<class_float>` sec **)**

指定两个动画（由它们的键所引用）之间的混合时间（以秒为单位）。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_set_method_call_mode:

.. rst-class:: classref-method

void **set_method_call_mode** **(** :ref:`AnimationMethodCallMode<enum_AnimationPlayer_AnimationMethodCallMode>` mode **)**

用于向后兼容。见 :ref:`AnimationCallbackModeMethod<enum_AnimationMixer_AnimationCallbackModeMethod>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_set_process_callback:

.. rst-class:: classref-method

void **set_process_callback** **(** :ref:`AnimationProcessCallback<enum_AnimationPlayer_AnimationProcessCallback>` mode **)**

用于向后兼容。见 :ref:`AnimationCallbackModeProcess<enum_AnimationMixer_AnimationCallbackModeProcess>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_set_root:

.. rst-class:: classref-method

void **set_root** **(** :ref:`NodePath<class_NodePath>` path **)**

用于向后兼容。见 :ref:`AnimationMixer.root_node<class_AnimationMixer_property_root_node>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_AnimationPlayer_method_stop:

.. rst-class:: classref-method

void **stop** **(** :ref:`bool<class_bool>` keep_state=false **)**

停止当前播放的动画。动画位置被重置为 ``0``\ ，\ ``custom_speed`` 被重置为 ``1.0``\ 。另见 :ref:`pause<class_AnimationPlayer_method_pause>`\ 。

如果 ``keep_state`` 为 ``true``\ ，则动画状态不会在视觉上更新。

\ **注意：**\ 方法/音频/动画播放轨道不会被该方法处理。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
