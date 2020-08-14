

根据各位建议加上了这部分内容，我暂时只是给出了两个资源，后续可能会对重要的点进行总结，然后更新在这里，如果你总结过这类东西，欢迎与我联系！

- **阿里巴巴Java开发手册（详尽版）** <https://github.com/alibaba/p3c/blob/master/阿里巴巴Java开发手册（详尽版）.pdf>
- **Google Java编程风格指南：** <http://www.hawstein.com/posts/google-java-style.html>

## 针对阿里Java开发手册特别注意
- 日期格式化时，传入 pattern 中表示年份统一使用小写的 y
> "yyyy-MM-dd HH:mm:ss" 中 HH 24小时制，hh 12小时制

- 判断所有集合内部的元素是否为空，使用 isEmpty()方法，而不是 size()==0 的方式
> 在某些集合中，前者的时间复杂度为 O(1)，而且可读性更好。

- 在使用 Collection 接口任何实现类的 addAll()方法时，都要对输入的集合参数进行
  NPE 判断。