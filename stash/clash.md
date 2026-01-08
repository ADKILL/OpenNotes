<!--
本文归属项目：`clash`
本文属性信息：|**clash**|S|valid|doing|undo|
本文修订状态：
草稿 20260108
-->


### 1.软件介绍

|软件名称|clash|
|:---:|:---:|
|所属国家|中国|
|软件类别| 实际生产| 
|有无插件| 没有|  
|配套软件| 没有|
|习得方式| 自学| 
|掌握情况| 优秀|  
|受众情况| 小众|  
|有无更新| 没有| 
|未来发展| 一般|
|软件版本| V2.5.4.foss|
|软件作用| 1.<br>2.<br>3.|
|软件评价||
|备注信息|1.<br>2.<br>3.|

### 2.软件获取及安装

#### 2.1 软件获取

#### 2.2 软件安装

### 3.软件使用教程及心得体会

#### 3.1 作为广告拦截器的yaml文件配置

1. yaml文件获取

 - 打开`clash`
 - (点击`运行中`按钮停止软件运行)
 - 点击`配置`按钮进入配置页面1
 - 点击右侧`⁝`
 - 点击下方`编辑`进入配置页面2
 - 点击`浏览文件`进入文件界面
 - 点击右侧`⁝`
 - 点击下方`导出`，将`配置文件.yaml`文件保存到手机根目录

2. yaml文件内容

```yaml文件内容
port: 7890
socks-port: 7891
allow-lan: false
mode: rule
log-level: info

proxies:
  - name: DIRECT
    type: direct

proxy-groups:
  - name: PROXY
    type: select
    proxies:
      - DIRECT

rules:

############################
# ❌ 禁止访问的域名
############################
#番茄免费小说
- DOMAIN,example.com,REJECT
- DOMAIN,mktm.jd.com,REJECT
- DOMAIN,example.com,REJECT
- DOMAIN,example.com,REJECT
- DOMAIN,example.com,REJECT
- DOMAIN,example.com,REJECT
- DOMAIN-SUFFIX,ads.example.net,REJECT
- DOMAIN-SUFFIX,zijieapi.com,REJECT
- DOMAIN-SUFFIX,bytedanceapi.com,REJECT
- DOMAIN-SUFFIX,dig.bdurl.net,REJECT
- DOMAIN-SUFFIX,byteimg.com,REJECT
- DOMAIN-SUFFIX,snssdk.com,REJECT
- DOMAIN-SUFFIX,vegslb.com,REJECT
#- DOMAIN-SUFFIX,douyinpic.com,REJECT 小说内容加载
#- DOMAIN-SUFFIX,ecombdapi.com,REJECT 小说内容加载
- DOMAIN-SUFFIX,ecombdimg.com,REJECT
- DOMAIN-SUFFIX,douyinliving.com,REJECT
- DOMAIN-SUFFIX,douyincdn.com,REJECT


############################
# ❌ 禁止访问的 IP / IP 段
############################
- IP-CIDR,1.2.3.4/32,REJECT,no-resolve
- IP-CIDR,8.8.8.0/24,REJECT,no-resolve

############################
# 其余全部放行
############################
- MATCH,DIRECT

```

3. yaml文件更新

 - 打开`clash`
 - (点击`运行中`按钮停止软件运行)
 - 点击`配置`按钮进入配置页面1
 - 点击正在使用的配置文件右侧的`⁝`
 - 点击下方`编辑`进入配置页面2
 - 点击`浏览文件`进入文件界面
 - 点击正在使用的配置文件右侧的`⁝`
 - 点击下方`导如`，选中手机根目录下修改过的`配置文件.yaml`文件导入
 - 返回上一层
 - 点击右上角保存按钮
 - 返回主页面
 - 点击`已停止`按钮启动软件运行

### 4.软件疑难解答

### 5.其它附件信息

#### 5.1 配置文件详解
#### 5.2 本人文件配置
#### 5.3 未分类附件



#### 图片插入链接模板

![*](https://github.com/ADKILL/ImageHub/blob/bda69bf17ea00fbc4e86a76793e10a792ea85d73/headface/folder.jpg?raw=true)

![*](https://raw.githubusercontent.com/ADKILL/ImageHub/main/headface/folder.jpg)