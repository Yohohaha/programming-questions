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