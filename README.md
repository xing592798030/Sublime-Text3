#  Sublime Text3 使用Package Control安装插件报错问题

当使用Package Control安装插件时，有时候会遇到如下错误：

```text
Package Control 

There are no packages available for installation 

Please see https://packagecontrol.io/docs/troubleshooting for help
```

<img src="D:\Typora\image\sublime_error.png" alt="sublime_error"  />

这是由于国内无法访问 <https://packagecontrol.io/> 的缘故，采取以下措施可以解决该问题。

## 1. 本地使用 channel_v3.json 

1. 从官网 <https://packagecontrol.io/channel_v3.json> （如果官网打不开可以到[文末下载](https://pan.baidu.com/s/16Tm1ckt6k_mdRJijaaHEFA "channel_v3.json")，提取码:iq3i ）下载最近版本 channel_v3.json 文件，放到指定目录，例如：D:\Sublime\patch
2. 点击 Preferences > Package Settings > Package Control > Settings - User
3. 在文本开头添加以下代码：`"channels": ["D:/Sublime/patch/channel_v3.json"],`

## 2. 直接使用网上的 channel_v3.json

1. 点击 Preferences > Package Settings > Package Control > Settings - User
2. 将 channel_v3.json 保存在网上，例如Github等
3. 在文本开头添加以下代码：

```text
"channels": ["https://github.com/xing592798030/Sublime-Text3/blob/master/channel_v3.json"],
```





**channel_v3.json 下载地址：**

链接：https://pan.baidu.com/s/16Tm1ckt6k_mdRJijaaHEFA

提取码：iq3i 
