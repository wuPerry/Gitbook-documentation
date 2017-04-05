# 个性化配置

除了修改书籍的主题外，还可以通过配置`book.json`文件来修改 gitbook 在编译书籍时的行为，例如：修改书籍的名称，显示效果等等。

#### 一：在线配置

在线编辑可以打开settings可以配置Title，description，topic等信息。勾选E-book选项可以在线导出pdf，mobi，epub。

#### 二：book.json配置

gitbook 在编译书籍的时候会读取书籍源码顶层目录中的`book.js`或者`book.json`，这里以`book.json`为例，参考[gitbook 文档](https://toolchain.gitbook.com/config.html)可以知道。

#### 三：插件

gitbook的默认插件：

\* highlight

\* search

\* sharing

\* font-settings

\* livereload

配置插件：

添加插件gitbook-plugin-image-captions
```
"plugins": [
    "image-captions"
]
```



