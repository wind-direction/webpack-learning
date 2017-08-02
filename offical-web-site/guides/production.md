# 生产环境构建

## 自动方式
下面两种方式是等效的：
- `webpack -p`
- `webpack --optimize-minimize --define process.env.NODE_ENV="'production'"`

会进行的操作：
- `UglifyJsPlugin`进行JS文件压缩
- `LoaderOptionsPlugn`
- 这是NodeJs的环境变量，触发某些packaege包，以不同的方式进行编译

## JS 文件压缩

自带了`UglifyJsPlugin`。

## Source Maps

运行基准测试(benchmark tests)

支持七种类型的source map[@devtool](https://doc.webpack-china.org/configuration/devtool/#devtool)

## Node 环境变量

会通过在插件列表中，调用`DefinePlugin`插件。
而`DefinePlugin`会在原始的源码中，执行查找和替换操作。将`process.env.NODE_ENV`替换成配置的参数，并且最终通过UglifyJs等价替换掉。

## 手动方式

### 简单方式 
