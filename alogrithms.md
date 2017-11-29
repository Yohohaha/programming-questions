- 去重

  - 比较元素索引是否是第一个索引
    ```python
    [x for idx, x in enumerate(l) if idx == l.index(x)]
    ```

