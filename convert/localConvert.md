# 本地导出

1. ##### 安装转换工具[Calibre application](https://calibre-ebook.com/download)，再执行

   ```
   npm install calibre -g
   ```
2. ##### 安装引用的插件[gitbook-plugin-image-captions](https://plugins.gitbook.com/plugin/image-captions),添加新插件之间需要运行gitbook install来安装新的插件

   ```
   gitbook install gitbook-plugin-image-captions
   ```

   \*如果安装不成功可以直接下载插件放到gitbook的安装文件下，全局安装的路径一般为  
   路径1：C:\Users\admin\AppData\Roaming\npm\node\_modules\gitbook\node\_modules

   但是在实现过程中发现gitbook引用的配置路径为  
   路径2：C:\Users\admin.gitbook\versions\3.2.2\node\_modules，所以如果正常步骤执行不成功的话把路径1  
    node\_modules下的文件全部拷贝到路径2的node\_modules。

3. ##### 导出的命令

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

   为了方便，先将目录切换到书籍的目录。步骤如下\(我的书籍路径 G:\gitbooks\wuperry\)：  
   一.“win+R”输入cmd打开cmd命令窗口  
   ![](/assets/import19.png)  
   二.在命令窗口输入“cd G:\gitbooks\wuperry”，回车再输入"g:"就会切换到G:\gitbooks\wuperry的目录下。  
   ![](/assets/import20.png)

   * ###### html

     在执行生成html命令后，会在书籍文件里边生成一个\_book的文件夹。

     ![](/assets/import13.png)

   * ###### pdf

     ```
     $ gitbook pdf gitbook-documentation  gitbook-documentation.pdf
     # gitbook-documentation是书籍文件；book.pdf是导出后的pdf文件，可以自己命名和定义路径
     ```

     在执行生成pdf命令后，会默认生成book.pdf的文件。

     ![](/assets/import14.png)



