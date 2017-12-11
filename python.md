- 列表获取索引的方法

  - ```python
    for idx, i in enumerate(l):
        i = l[idx]
    ```

- 从列表中提取指定索引

  - ```python
    [i for idx, i in enumerate(l) if idx in indices]
    ```

- 列表切片
  - `l[:]`和`l[::]`都表示复制列表
  - `l[0:6]`表示从索引0到索引6
  - `l[0:6:1]`表示从索引0到索引6每隔**0**个取一个
  - `l[0:6:2]`表示从索引0到索引6每隔**1**个取一个

- python3中的正则表达式字符串需要加r吗？

  - 不需要

- sys模块中args的意思？

  - args代表脚本运行时的命令行参数，`args[0]`始终表示程序名，例：test.py

- python中的私有变量？

  - python的私有变量定义方法为在变量名前面加`_`或`__`

- 如何获取python的包搜索路径(类似于java中的classpath)？

  - ```python
    import sys
    sys.path
    ```

  - 添加自定义的path路径

    ```python
    import sys
    sys.path.append('/user/somebody/mypythonpath')
    ```

- 判断函数类型的方法？

  - 使用types模块中定义的常量
    ```python
    import types
    def fn():
    	pass
    type(fn) == types.FunctionType
    ```

  - 使用`isinstance`判断，使用方法和type一样，而且`isinstance`还可以判断多个

- 如何限定一个类的属性定义？

  - 使用`__slots__`

- 对于python中魔法方法的理解？

  - python中的魔法方法类似于java中的通用接口，如`Clonable`、`Closable`等或java的Object类中定义的`toString()`等，然后再对其做一些语法上面的转化，类比java中对`toString()`方法在打印的时候做出的转化