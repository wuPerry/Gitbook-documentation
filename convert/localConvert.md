# 本地导出

1. 安装转换工具[Calibre application](https://calibre-ebook.com/download)，再执行

   ```
   npm install calibre -g
   ```

2. 安装引用的插件[gitbook-plugin-image-captions](https://plugins.gitbook.com/plugin/image-captions),添加新插件之间需要运行gitbook install来安装新的插件

   ```
   gitbook install gitbook-plugin-image-captions
   ```
   *如果安装不成功可以直接下载插件放到gitbook的安装文件下，全局安装的路径一般为
   路径1：C:\Users\admin\AppData\Roaming\npm\node_modules\gitbook\node_modules
   
   但是在实现过程中发现gitbook引用的配置路径为
   路径2：C:\Users\admin\.gitbook\versions\3.2.2\node_modules，所以如果正常步骤执行不成功的话把路径1
    node_modules下的文件全部拷贝到路径2的node_modules。
 3. 导出的命令
   ```
   # html
   $ gitbook serve
   
   # Generate a PDF file
   $ gitbook pdf ./ ./mybook.pdf

   # Generate an ePub file
   $ gitbook epub ./ ./mybook.epub

   # Generate a Mobi file
   $ gitbook mobi ./ ./mybook.mobi
   ```


