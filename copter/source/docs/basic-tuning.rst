.. _basic-tuning:

============
基本调参
============

本文档涵盖了基本的横滚、俯仰和油门调参。

概述
========

在你首次试飞后，你可能会发现你的无人机并未按你所预想的那样对遥控输入作出响应，或者难以维持对无人机的控制。如果你熟悉PID控制器，请查阅 :ref:`advanced tuning guide here <tuning>` 。如果你是位经验丰富的飞手，试试 :ref:`the autotune feature <autotune>`。
本页面包含 Mission Planner 和 APM Planner 的基本调参，其将复杂的调参过程简化为了几个简单滑块。这是对于新手来说最好的调参方法。

横滚和俯仰调参
=====================

使用 :ref:`telemetry radio <common-telemetry-landingpage>` 是进行现场调参最简单的方法。带着以下问题进行首飞：

-  无人机在横滚和俯仰上响应如何？是否比你想要的更迟缓或者更激烈？
-  无人机悬停时，油门在什么位置？它在油门中位时悬停，还是高于或低于中位？
-  推油门时，无人机以多大的速率进行加速？它的上升速度是否比你想要的更高或更低？

将数传电台地面端连接到电脑，启动地面站，选择正确的COM口后点击连接。你应当能在飞行数据界面看到实时数据。选中Config/Tuning和Basic Tuning以开始调参。

首先从页面顶上的横滚/俯仰滑块开始。如果你发现到你的无人机的横滚和俯仰太迟缓，将滑块向左移动一格。相反，如果你发现到你的无人机的横滚和俯仰太激烈，将滑块向右移动一格。重复飞行测试来确认你的调整是否有效。重复这一过程，直到你对无人机的横滚和俯仰响应满意为止。

.. image:: ../images/apm-planner-basic-tuning2.png
    :target: ../_images/apm-planner-basic-tuning2.png

.. image:: ../images/mission-planner-basic-tuning.png
    :target: ../_images/mission-planner-basic-tuning.png

油门调参
===============

底部的两个滑块能够调试油门。调整 Throttle Hover 滑块，如果无人机在油门中位以上悬停，将滑块向左移动一格。如果无人机在油门中位以下悬停，将滑块向右移动一格。边调整边测试，直至无人机在油门中位时悬停。务必测试你的每一次调整。

将 Throttle Accel 或者 Climb Sensitivity 滑块向右移动以使无人机上升更迅猛，或者向左移动以使其上升更平缓。每次调整后进行测试评估。
