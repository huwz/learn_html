HTML 学习笔记
=============

.. important::
 "I often use FrontPage, but although it is one of the best, it never seems to do just what I want for some applications. I just as often use jsEditor, because it gives me a lot more control. It would be silly not to use the tools which make our job easier, but we should not be a slave to them. We can only master the tools for HTML by learning a bit about it! I think that understanding HTML is essential, but that is just my opinion. "

基础知识
--------

* 后缀: **html** 或 **htm**
* 标题标签：
  
  tag       说明
   *h1*    一级标题
   *h2*    二级标题
   *h3*    三级标题
   *h4*    四级标题
   *h5*    五级标题
   *h6*    六级标题
  
* 段落
  
  *<p>*

  .. note:: 另起一段不是用回车换行符实现，只能用 <p> 标签

* 换行
  
  *<br/>*

  .. note:: 换行也不是回车换行完成的，需要 <br/> 标签
  
* 注释  ``<!-- comments her -->``
  
字体变换
--------
  
+--------+------+
| 转换   | 标签 |
+========+======+
| 加粗   | <b>  |
+--------+------+
| 下划线 | <u>  |
+--------+------+
| 斜体   | <i>  |
+--------+------+

.. note:: 这些标签可以自由组合，效果相互叠加

<body>
------

+------------+-----------------------+
| 属性       | 值                    |
+============+=======================+
| bgcolor    | "<colorname>/#xxxxxx" |
+------------+-----------------------+
| background | "<picture uri>"       |
+------------+-----------------------+


<hr>
----

水平规则

+-------+------------------------+
| 属性  | 默认值                 |
+=======+========================+
| size  | 2(pixels)              |
+-------+------------------------+
| width | 100(%)                 |
+-------+------------------------+
| color | 白色 (#FFFFFF / White) |
+-------+------------------------+
| align | CENTER(LEFT / RIGTH)   |
+-------+------------------------+

.. note:: 不区分大小写，
 属性值都需要双引号包围，下同

<A>
---


+--------------+-----------------+--------------------------------+
| 属性         | 值              | 含义                           |
+==============+=================+================================+
| href         | url/#<tag_name> | 链接地址/跳转 tag              |
+--------------+-----------------+--------------------------------+
| content      | string          | 链接内容，为空时链接内容为 url |
+--------------+-----------------+--------------------------------+
| [body] vlink | colorname       | 点击过的链接颜色               |
+--------------+-----------------+--------------------------------+
| [body] alink | colorname       | 正点击的链接颜色               |
+--------------+-----------------+--------------------------------+
| [body] link  | colorname       | 未点击的链接颜色               |
+--------------+-----------------+--------------------------------+
| title        | string          | 光标停留在链接上时提示内容     |
+--------------+-----------------+--------------------------------+
| name         | string          | 定义一个跳转 tag               |
+--------------+-----------------+--------------------------------+

发送邮件

``<a href="mailto:yourmail@***.com?subject=<string>">link nanme</a>``

.. note:: 
 在引用 tag 跳转时，最好把文件名带上，比如 ``<a href="jmp.html#top">go to the top</a>``

<img>
-----

+--------+-------------------------------+
| 属性   | 说明                          |
+========+===============================+
| src    | 图片路径                      |
+--------+-------------------------------+
| alt    | 图片链接文字                  |
+--------+-------------------------------+
| border | 图片边框，默认 "0" 表示无边框 |
+--------+-------------------------------+
| align  | 周围文字的对齐方式            |
+--------+-------------------------------+
| width  | 图片宽度                      |
+--------+-------------------------------+
| height | 图片高度                      |
+--------+-------------------------------+

列表
----


.. note:: <br CLEAR="all"> 表示不被文字包围
