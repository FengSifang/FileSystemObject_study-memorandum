# FileSystemObject_study-memorandum
A memoran worked by Javascript(FileSystemObject)
#### 介绍
突然发现js可以操作目录，所以写了个简单的demo，所以就有了这个记事本，因为原生js写的不是很好，还想写成一个文件，所以直接把jquery粘在了里面。

#### 环境
限IE，windows（路径写的的windows，没做版本测试）
测试环境win10 ie11

#### 实现功能
实现了基本的增删改查
运行后会在d盘生成一个note文件夹，文件夹中生成conf.ini文件，和recycle文件夹。
运行后页面依次为笔记本，文章，和内容
每添加一个文章会生成一个txt文件用来记录内容
删除后文件会移动到recycle，30天以后自动移除

#### 目录结构
+note
+---recycle
+------delete.txt
+---conf.ini
+---content.txt

#### 使用说明
content是个textarea，里面的内容可以转为html添加在原来的位置
双击内容可依靠html标签编辑
如果需要编辑全部内容 可以点顶端button

#### Description
I write this easy demo when I found JS can operate files. I put jquery in this file because of I'm not good at JS and I hope everything in one file.

#### Environment
Only in IE windows
my test enviroment is IE11 AND win10

#### How to use it
When you open note.html by IE, this file will generate a folder which name is note in D:\(you can change it in file). A file conf.ini and another folder recycle in note.
Then you can see the html seperated by 3 parts. Click button to add. First and second parts will generate a tree in conf.ini, Third part will generate a file in note. When you delete it, I move Third part file into folder recycle and delete the file after 30 days.
You can write html into third part And edit short html by double click content. 