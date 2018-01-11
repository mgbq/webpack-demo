# webpack-test

0.1、安装webpack

首先你需要安装Node.js，点击打开Node.js下载页面。安装完Node.js后，会自带npm包管理器。

npm install webpack -g

这个命令将安装最新版本的webpack（全局)

webpack -v

0.2、查看当前webpack版本

执行命令：

以下执行webpack命令时，指在对应文件夹下，通过控制台执行命令。

快速抵达对应目录的控制台（win）：

在对应目录下，按住 shift，然后点击鼠标右键，在弹窗里选择在此处打开命令窗口即可启用

webpack hello.js hello.bundle.js

0.3、把hello.js文件打包为hello.bundle.js

hello.js里面也可以有css和其他的js

0.4、导入了css打包的时候得指定文件类型才能打

webpack hello.js hello.bundle.js --module-bind "css=style-loader!css-loader"

0.5，频繁修改文件频繁打包很麻烦，用下面命令打包修改代码就不用打包了

webpack hello.js hello.bundle.js --module-bind "css=style-loader!css-loader" --watch

优点，index页面只需要引入一个文件即可 
注意要点

第一，安装的时候先要全局安装webpack 就是加上-g。

第二，文件名字不能重复webpack名字。

第三，windown下 更改”css=style-loader!css-loader!” 是双引号
