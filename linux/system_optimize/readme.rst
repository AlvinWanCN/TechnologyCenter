linux optimize
#########################

.. contents::

关机提示： a stop job is running for....
``````````````````````````````````````````````

 关机提示： a stop job is running for... 太耗时，

一、现象
-----------------

Linux关机或重启时提示A stop job is running for ..


导致关机慢。


二、解决方法
-------------------

编辑/etc/systemd/system.conf


修改下面两个变量为：


DefaultTimeoutStartSec=10s
DefaultTimeoutStopSec=10s
执行：systemctl daemon-reload
文章标签： kali linux linux
