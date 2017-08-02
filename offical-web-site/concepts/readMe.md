# [概念](https://doc.webpack-china.org/concepts/)

webpack 是一个

- 模块打包器`module bundler`
- 会递归构建一个依赖关系图`dependency graph`

## [入口(entry)](https://doc.webpack-china.org/concepts/#-entry-)

入口点(*entry point*) 是依赖关系图的起点。

由配置对象的`entry`属性定义入口。

## [出口(output)](https://doc.webpack-china.org/concepts/#-output-)

告诉webpack 在哪里打包应用程序。

由配置对象的`output`属性定义。

## [加载器(loader)](https://doc.webpack-china.org/concepts/#loader)

在webpack中所有资源都是模块。

webpack 自身职能理解javascript。

加载器(Loader)在文件被添加到依赖图中时，将其转换成模块。

两个属性：

- `test`: 识别应该被对应的loader进行转换的文件
- `use`: 转换这些文件，从而使其加到依赖图中


## [插件(plugin)](https://doc.webpack-china.org/concepts/#-plugins-)

插件用于在`compilation`和`chunk`阶段，对模块进行额外的操作，这些操作可以是插件自带的，也可以是用户自定义的。

使用时：

- 需要`require`进来
- 添加到`plugins`数组中

## 单词表

|英文|中文|
|:---|:---|
|依赖关系图| dependency graph |
|资源| assets |
|归拢后的代码| bundled code
|项目生成 | emit |
|识别| identify |
|转换| transform|
