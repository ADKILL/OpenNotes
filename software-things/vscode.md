<!--
本文归属项目：`vscode`
本文修订状态：草稿
-->


### 1. introduction

  软件名称：vscode  
  所属国家：美国<input type="checkbox" checked> 英国<input type="checkbox"> 日本<input type="checkbox"> 中国<input type="checkbox"> 其他<input type="checkbox">  
  软件类别：代码编程<input type="checkbox" checked> 工农生产<input type="checkbox"> 学术研究<input type="checkbox">  
  有无插件：有的<input type="checkbox" checked> 没有<input type="checkbox">  
  配套软件：有的<input type="checkbox"> 没有<input type="checkbox" checked>  
  习得方式：自学<input type="checkbox" checked> 课堂<input type="checkbox"> 培训<input type="checkbox"> 他人传授<input type="checkbox">  
  掌握情况：优秀<input type="checkbox"> 良好<input type="checkbox"> 一般<input type="checkbox" checked>  
  受众情况：大众<input type="checkbox" checked> 小众<input type="checkbox"> 很小众<input type="checkbox">  
  有无更新：有的<input type="checkbox" checked> 没有<input type="checkbox">  
  未来发展：优秀<input type="checkbox" checked> 良好<input type="checkbox"> 一般<input type="checkbox"> 过时<input type="checkbox">  
  软件作用：`文件编辑` `代码编写` `程序调试`

### 2. installation

### 3. instruction

### 4. troubleshooting

1. 软件都是英文，看着不方便  
 
- 点击左侧`扩展(ctrl+shift+x)`按钮，进入扩展商店，搜索框中键入<em>**chinese**</em>，在下方的提供的选项中点击安装`chinese language pack for visual studio code`，重启vscode，显示界面变成中文  

2. 用vscode推送总是失败，用github总能成功   

- 直接给git添加代理，代码如下：  
```
git config --global http.proxy http://127.0.0.1:9981
git config --global https.proxy https://127.0.0.1:9981
```

3. vscode的扩展商店打不开，可能与`q2`中的代理设置有关系

- `q2`中只是给git添加了代理，vscode没添加，所以不行
- `ctrl+,`，在弹出窗口的文本框内键入`proxy`，选择弹出的`Http: Proxy`选项卡的输入框内键入`http://127.0.0.1:9981`，关闭页面，重启vscode，问题解决
- 之前没添加代理也能打开，真是奇了怪了