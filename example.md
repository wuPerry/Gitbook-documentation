# 案例

### 本地（window）：

##### 步骤一：安装nodejs

安装教程参考以下链接:

[http://www.runoob.com/nodejs/nodejs-install-setup.html](http://www.runoob.com/nodejs/nodejs-install-setup.html)

##### 步骤二：安装gitbook

打开运行,输入以下命令：

```
npm install -g gitbook-cli
```

![](/assets/import15.png)

检查安装：

在运行窗口输入以下命令检查gitbook是否安装成功

```
gitbook -V
```

##### 步骤三：安装gitbook的相关插件

```
gitbook install gitbook-plugin-image-captions
```

插件路径[gitbook-plugin-image-captions](https://plugins.gitbook.com/plugin/image-captions)  
\*如果安装不成功可以直接下载插件放到gitbook的安装文件下，全局安装的路径一般为  
路径1：C:\Users\admin\AppData\Roaming\npm\node\_modules\gitbook\node\_modules

但是在实现过程中发现gitbook引用的配置路径为  
路径2：C:\Users\admin.gitbook\versions\3.2.2\node\_modules，所以如果正常步骤执行不成功的话把路径1  
node\_modules下的文件全部拷贝到路径2的node\_modules

