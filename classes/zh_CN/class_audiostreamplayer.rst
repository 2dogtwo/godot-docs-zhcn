:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/AudioStreamPlayer.xml.

.. _class_AudioStreamPlayer:

AudioStreamPlayer
=================

**继承：** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

播放音频，不考虑所处位置。

.. rst-class:: classref-introduction-group

描述
----

以非位置方式支持播放音频流。

要在位置上播放音频，请使用 :ref:`AudioStreamPlayer2D<class_AudioStreamPlayer2D>` 或 :ref:`AudioStreamPlayer3D<class_AudioStreamPlayer3D>` 而不是 **AudioStreamPlayer**\ 。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`音频流 <../tutorials/audio/audio_streams>`

- `2D Dodge The Creeps 演示 <https://godotengine.org/asset-library/asset/515>`__

- `音频设备切换演示 <https://godotengine.org/asset-library/asset/525>`__

- `音频生成器演示 <https://godotengine.org/asset-library/asset/526>`__

- `音频麦克风录音演示 <https://godotengine.org/asset-library/asset/527>`__

- `音频频谱演示 <https://godotengine.org/asset-library/asset/528>`__

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`bool<class_bool>`                            | :ref:`autoplay<class_AudioStreamPlayer_property_autoplay>`           | ``false``     |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`StringName<class_StringName>`                | :ref:`bus<class_AudioStreamPlayer_property_bus>`                     | ``&"Master"`` |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`int<class_int>`                              | :ref:`max_polyphony<class_AudioStreamPlayer_property_max_polyphony>` | ``1``         |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` | :ref:`mix_target<class_AudioStreamPlayer_property_mix_target>`       | ``0``         |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`pitch_scale<class_AudioStreamPlayer_property_pitch_scale>`     | ``1.0``       |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`bool<class_bool>`                            | :ref:`playing<class_AudioStreamPlayer_property_playing>`             | ``false``     |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`AudioStream<class_AudioStream>`              | :ref:`stream<class_AudioStreamPlayer_property_stream>`               |               |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`bool<class_bool>`                            | :ref:`stream_paused<class_AudioStreamPlayer_property_stream_paused>` | ``false``     |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+
   | :ref:`float<class_float>`                          | :ref:`volume_db<class_AudioStreamPlayer_property_volume_db>`         | ``0.0``       |
   +----------------------------------------------------+----------------------------------------------------------------------+---------------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                             | :ref:`get_playback_position<class_AudioStreamPlayer_method_get_playback_position>` **(** **)**           |
   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
   | :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` | :ref:`get_stream_playback<class_AudioStreamPlayer_method_get_stream_playback>` **(** **)**               |
   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | :ref:`has_stream_playback<class_AudioStreamPlayer_method_has_stream_playback>` **(** **)**               |
   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
   | void                                                  | :ref:`play<class_AudioStreamPlayer_method_play>` **(** :ref:`float<class_float>` from_position=0.0 **)** |
   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
   | void                                                  | :ref:`seek<class_AudioStreamPlayer_method_seek>` **(** :ref:`float<class_float>` to_position **)**       |
   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
   | void                                                  | :ref:`stop<class_AudioStreamPlayer_method_stop>` **(** **)**                                             |
   +-------------------------------------------------------+----------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

信号
----

.. _class_AudioStreamPlayer_signal_finished:

.. rst-class:: classref-signal

**finished** **(** **)**

当音频停止播放时发出。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

枚举
----

.. _enum_AudioStreamPlayer_MixTarget:

.. rst-class:: classref-enumeration

enum **MixTarget**:

.. _class_AudioStreamPlayer_constant_MIX_TARGET_STEREO:

.. rst-class:: classref-enumeration-constant

:ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` **MIX_TARGET_STEREO** = ``0``

音频将只在第一个声道中播放。

.. _class_AudioStreamPlayer_constant_MIX_TARGET_SURROUND:

.. rst-class:: classref-enumeration-constant

:ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` **MIX_TARGET_SURROUND** = ``1``

音频将在所有环绕声声道中播放。

.. _class_AudioStreamPlayer_constant_MIX_TARGET_CENTER:

.. rst-class:: classref-enumeration-constant

:ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` **MIX_TARGET_CENTER** = ``2``

音频将在第二个声道中播放，通常位于中央。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_AudioStreamPlayer_property_autoplay:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **autoplay** = ``false``

.. rst-class:: classref-property-setget

- void **set_autoplay** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_autoplay_enabled** **(** **)**

如果为 ``true``\ ，在添加到场景树时将播放音频。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_bus:

.. rst-class:: classref-property

:ref:`StringName<class_StringName>` **bus** = ``&"Master"``

.. rst-class:: classref-property-setget

- void **set_bus** **(** :ref:`StringName<class_StringName>` value **)**
- :ref:`StringName<class_StringName>` **get_bus** **(** **)**

这个音频在哪个总线上播放。

\ **注意：**\ 设置这个属性时，请记住它并不会对给定的名称是否与现有总线匹配进行校验。这是因为音频总线布局可以在设置这个属性后再加载。如果这个给定的名称在运行时无法解析，就会回退到 ``"Master"``\ 。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_max_polyphony:

.. rst-class:: classref-property

:ref:`int<class_int>` **max_polyphony** = ``1``

.. rst-class:: classref-property-setget

- void **set_max_polyphony** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_max_polyphony** **(** **)**

该节点可以同时播放的最大声音数。达到此值后，播放额外的声音将切断最旧的声音。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_mix_target:

.. rst-class:: classref-property

:ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` **mix_target** = ``0``

.. rst-class:: classref-property-setget

- void **set_mix_target** **(** :ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` value **)**
- :ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` **get_mix_target** **(** **)**

如果音频配置有两个以上的扬声器，则设置目标通道。见 :ref:`MixTarget<enum_AudioStreamPlayer_MixTarget>` 常量。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_pitch_scale:

.. rst-class:: classref-property

:ref:`float<class_float>` **pitch_scale** = ``1.0``

.. rst-class:: classref-property-setget

- void **set_pitch_scale** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_pitch_scale** **(** **)**

音频的音高和节奏，作为音频样本的采样率的倍数。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_playing:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **playing** = ``false``

.. rst-class:: classref-property-setget

- :ref:`bool<class_bool>` **is_playing** **(** **)**

如果为 ``true``\ ，则播放音频。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_stream:

.. rst-class:: classref-property

:ref:`AudioStream<class_AudioStream>` **stream**

.. rst-class:: classref-property-setget

- void **set_stream** **(** :ref:`AudioStream<class_AudioStream>` value **)**
- :ref:`AudioStream<class_AudioStream>` **get_stream** **(** **)**

要播放的 :ref:`AudioStream<class_AudioStream>` 对象。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_stream_paused:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **stream_paused** = ``false``

.. rst-class:: classref-property-setget

- void **set_stream_paused** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_stream_paused** **(** **)**

如果为 ``true``\ ，则播放会暂停。你可以通过将 :ref:`stream_paused<class_AudioStreamPlayer_property_stream_paused>` 设置为 ``false``\ 来恢复它。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_property_volume_db:

.. rst-class:: classref-property

:ref:`float<class_float>` **volume_db** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_volume_db** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_volume_db** **(** **)**

音量，单位为 dB。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_AudioStreamPlayer_method_get_playback_position:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_playback_position** **(** **)**

返回 :ref:`AudioStream<class_AudioStream>` 中的位置，单位为秒。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_method_get_stream_playback:

.. rst-class:: classref-method

:ref:`AudioStreamPlayback<class_AudioStreamPlayback>` **get_stream_playback** **(** **)**

返回与此 **AudioStreamPlayer** 关联的 :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` 对象。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_method_has_stream_playback:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has_stream_playback** **(** **)**

返回该 **AudioStreamPlayer** 是否能够返回 :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` 对象。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_method_play:

.. rst-class:: classref-method

void **play** **(** :ref:`float<class_float>` from_position=0.0 **)**

从给定的位置 ``from_position`` 播放音频，以秒为单位。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_method_seek:

.. rst-class:: classref-method

void **seek** **(** :ref:`float<class_float>` to_position **)**

设置音频的播放位置，以秒为单位。

.. rst-class:: classref-item-separator

----

.. _class_AudioStreamPlayer_method_stop:

.. rst-class:: classref-method

void **stop** **(** **)**

停止音频。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
