0301 Sphinx 工具学习
===============

Sphinx 是一个工具，它使得创建一个智能而美丽的文档变得简单。作者Georg Brandl，基于BSD许可证。
Sphinx 使用 reStructuredText 作为编写语言，也可以使用 Markdown + 拓展库的方式进行文档的编写。


安装
----------------
需要python3环境

.. code-block:: xml
    $ cd ~/DL/env_python3
    $ source env_python3/bin/activate
    $ pip3 install -U sphinx # Linux系统
    # or
    $sudo apt-get install python3-sphinx


常用语法
-------------

Subtitles are set with '-' and are required to have the same length 
of the subtitle itself, just like titles.

Lists can be unnumbered like:

 * Item Foo
 * Item Bar

Or automatically numbered:

 #. Item 1
 #. Item 2


Words can have *emphasis in italics* or be **bold** and you can define
code samples with back quotes, like when you talk about a command: ``sudo`` 
gives you super user powers!

表格

.. csv-table::
    :header:参数,类型,含义
    :widths:2,2,5

    test1,String,这里是测试的第一行
    test2,int,这里是测试的第二行

代码块

.. code-block:: xml

    public void test(){
        throws new Exception("this is a test");
    }

引用其他模块文件

点击跳转

建立第一个工程
----------------
直接命令行运行 ``sphinx-quickstart`` ，按照向导进行建立工程

.. image:: ../_static/tree.png

点击跳转

调用 :ref:`点击这里跳转<file.key>`

编译方式：

.. code-block:: xml

    $cd ~/Documents/sphinx_tutorial
    $make html

配置github环境
----------------

.. code-block:: xml

    git config --global user.email "zuisixian@mail.com"
    git config --global user.name "zuisixian"
    ssh-keygen -t rsa -C "zuisixian@mail.com"


官网资料
----------------
 #. https://www.sphinx-doc.org/en/master/devguide.html
 #. https://www.sphinx-doc.org/en/master/#confval-language
 #. https://www.cnblogs.com/Terrypython/p/10203332.html
 #. https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html
 #. https://www.sphinx-doc.org/en/master/#confval-language
 #. github: https://github.com/sphinx-doc/sphinx
 #. projects using Sphinx: https://www.sphinx-doc.org/en/master/examples.html
 #. getstarted: https://matplotlib.org/sampledoc/getting_started.html#installing-your-doc-directory



reference
----------------

 #. https://www.cnblogs.com/yqmcu/p/9837167.html
 #. https://blog.csdn.net/yeshennet/article/details/82595369