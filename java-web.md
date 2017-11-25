- 页面重定向和转发的url写法？

  - 页面重定向
  - 转发
    ```java
    req.getRequestDispatcher("/WEBINF/view/some.jsp").forward(req, resp);
    ```

- 文件上传
  - form表单写法
    ```html
    <form enctype="multipart/form-data" method="post">
        <input type="file" name="file" multiple="multiple"/>
        <input type="submit" value="提交"/>
    </form>
    ```
    其中`multiple="multiple"`表示上传多个文件
  - servlet注解
    ```java
    @MultipartConfig(
       fileSizeThreshold = 5_242_880,  // 文件大于5M则存为临时文件
       maxFileSize = 20_971_520,  // 单个文件大小最大为20M
       maxRequestSize = 41_943_040  // 本次请求的大小最大为40M，一次请求可以带有多个文件
    )
    ```
- jsp隐式变量
  - request和response
  - session
  - out -> outWriter，一般不使用它，而是直接在jsp中写文本
  - application -> ServletContext
  - config -> ServletConfig
  - pageContext
  - page -> 当前的Servlet对象
  - exception

