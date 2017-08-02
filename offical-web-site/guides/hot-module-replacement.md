# [模块热替换](https://doc.webpack-china.org/guides/hot-module-replacement/)

HMR: 允许在运行时更新各种模块，而无需进行完全刷新。

**注意**：HMR不适用于生产环境，应当只在开发环境中使用这个功能。

## 问题

当使用新代码对旧代码进行修补(patch)的时候，那些旧的实例就不会反映出来，除非我们以使用`module.hot.accept`的方式重新实例化他们。

## HMR 修改样式表

可以使用`style-loader`来实现模块热替换(Hot Module Replacement)。

## 其他代码框架


