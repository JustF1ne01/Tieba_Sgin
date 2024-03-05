# Tieba_Sgin

一个python脚本，可以实现百度贴吧签到，支持青龙面板运行只需要百度账号的BDUSS即可

引用项目: https://github.com/fanfan142/Tieba_Sgin.git


#### 修改后的功能：

1. 修改成变量方式
   export Tieba_BDUSS=""
2. 修改通知方式，去除只Server酱通知

#### 青龙面板使用

1. 青龙面板使用需要再python3中添加 pretty_errors 和 requests 依赖
2. 抓取百度贴吧Application中的Cookies BDUSS的value值
   ![image-20240302121449165](https://github.com/wq-h/pictures/blob/main/image-20240302121449165.png?raw=true)
3. 拉取命令
```shell
ql repo https://github.com/wq-h/Tieba_Sgin.git "Tieba_Sgin.py" "README.md" "sendNotify.py" "main"
```
