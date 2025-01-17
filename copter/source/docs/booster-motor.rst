.. _booster-motor:

=============
助推电机
=============

..  youtube:: RjjF_S69Ywk
    :width: 100%

Copter 3.6 （或更高版本）支持在机架中心安装额外的电机来提供额外升力。这一功能兼容所有的多旋翼机架（例如四轴，三轴，六轴，八轴，六轴十二旋翼）。上面的视频中使用一台 :ref:`内燃发动机 <common-ice>` 展示了这个功能，但此功能同样适用于电动机。

.. 注意::

   旋翼无人机暂不支持仅通过水平安装的电机而不倾斜无人机的方式进行移动 (`在这里提出改进要求 <https://github.com/ArduPilot/ardupilot/issues/10117>`__)。

调试
-------------

-  将助推电机的电调连接到飞控的一个输出口（例如 MAIN OUT 1 ~ 8 或者 AUX OUT 1 ~ 6）；
-  设置 SERVOx_FUNCTION = 81 为 "Boost Throttle" （ "x" 是输出口编号）；
-  可以设置 :ref:`MOT_BOOST_SCALE <MOT_BOOST_SCALE>` 为一个 0 到 5 之间的值，以根据输入到主电机的平均油门来调整助推电机输出。比例因数越大，助推电机的负载越高。 1 将设置助推油门等于主油门。主电机的输出将始终介于 ``SERVOx_MIN`` 和 ``SERVOx_MAX`` 的值之间（ "x" 是输出口编号）。
