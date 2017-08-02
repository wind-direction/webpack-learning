# [管理输出](https://doc.webpack-china.org/guides/output-management/)

`HtmlWebpackPlugin`用来解决入口点名称发生变更，而页面依然使用旧的名字的问题。

## [清理/dist文件夹](https://doc.webpack-china.org/guides/output-management/#-dist-)

- webpack 并不能追踪到哪些文件是实际在项目中用到的。
- 在每次构建前清理`/dist`目录是比较推荐的做法。

## [Manifest](https://doc.webpack-china.org/guides/output-management/#manifest)

- 通过`manifest`,webpack能够对*你的模块映射到bundle的过程*保持追踪。
