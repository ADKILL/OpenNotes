<!--
本文归属项目：`github`
本文属性信息：|**github**|S|valid|doing|undo|
本文修订状态：
草稿 20251129 25251203
-->


### 1.软件介绍

|软件名称|github|
|:---:|:---:|
|所属国家|美国|
|软件类别| 实际生产| 
|有无插件| 没有|  
|配套软件| 网页端<br>手机APP<br>桌面应用<br>vscode etc.|
|习得方式| 自学| 
|掌握情况| 一般|  
|受众情况| 大众|  
|有无更新| 有的| 
|未来发展| 优秀|
|软件版本| /|
|软件作用| 1.寻找代码应用<br>2.储存代码应用<br>3.作为图床使用等|
|软件评价|这是开源互联网真正的希望|
|备注信息|1.<br>2.<br>3.|

### 2.软件获取及安装

#### 2.1 软件获取

#### 2.2 软件安装

### 3.软件使用教程及心得体会

#### 3.1 作为图床使用时图片链接格式

注意：
1. 需要安装`github pull request`插件才能在vscode中实现图片的上传和复制链接操作
2. 不安装插件也可在github网站复制链接


#### 3.1.1 图片上传到github及vscode中的链接复制操作

1. 图片上传到github
   1. vscode 中切换到图片仓库
   2. 将图片复制粘贴到特定目录下
   3. 提交仓库更改到github
2. vscode中的链接复制操作
   1. 选中需要复制markdown格式链接的图片
   2. `右键`-->`共享`-->`将 github permalink 复制为 markdown`
   3. 将链接粘贴到需要位置，进行格式的修改

#### 3.1.2 直接从vscode复制的链接格式
```
  ![folder](https://github.com/ADKILL/ImageHub/blob/bda69bf17ea00fbc4e86a76793e10a792ea85d73/headface/folder.jpg?raw=true)
```
***注意：链接最前需要加上`!`，链接最后需要加上`?raw=true`字符串***
![folder](https://github.com/ADKILL/ImageHub/blob/bda69bf17ea00fbc4e86a76793e10a792ea85d73/headface/folder.jpg?raw=true)

#### 3.1.3 使用CDN加速节点的链接格式(pic-go图床上传的链接格式)
```
![folder](https://raw.githubusercontent.com/ADKILL/ImageHub/main/headface/folder.jpg)
```
***注意：该链接格式与图床软件没有任何关系，只要仓库里图片存在，手动生成该格式的链接就能正常访问***
![folder](https://raw.githubusercontent.com/ADKILL/ImageHub/main/headface/folder.jpg)

### 4.软件疑难解答

1. 在vscode里同时改动了很多文件，但又想每个文件单独提交，如何操作
   在`源代码管理`里选中要提交的文件(可以按住`control`键同时选中多个文件)，点击右侧`+`标志，文件进入暂存区，在上方`消息`栏输入提交信息，点击`提交`按钮，当前选中文件单独提交完成

### 5.其它附件信息

#### 5.1 配置文件详解
#### 5.2 本人文件配置
#### 5.3 未分类附件