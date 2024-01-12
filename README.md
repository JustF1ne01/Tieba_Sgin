# Tieba_Sgin
一个python脚本，可以实现百度贴吧签到，并通过Serve酱将详细签到结果推送到微信，支持青龙面板运行
可以使用青龙面板运行，只需要百度账号的BDUSS即可，使用Serve酱需要SendKey


#### 首先要先声明一下，我并不程序员，只是个iT从业者，各种东西都只是略懂一丢丢而已。

原脚本是小伙伴从吃灰的收藏夹挖出来的，原脚本作者是谁已经不知道到是谁了，原来脚本可以实现签到和消息推送，但是推送消息只会告诉你签到成功多少个，失败多少个这样，并不可以把签到的详细情况推送。
我使用AI和自己做琢磨做了一些修改。


### 修改后的功能：
1. 使用账号的BDUSS可以进行贴吧签到（废话）.
2. 使用Server酱可以推送签到结果到微信（修改更改了推送内容，比原有脚本更详细）
   （1）添加了签到成功的贴吧、签到失败的贴吧、已经签到的贴吧3个列表
   （2）签到成功的贴吧添加了是第几个签到的数据
![图片](https://github.com/yingfeng-i/Tieba_Sgin/assets/18555737/b1491946-b09c-4227-9282-236275056676)

3. 限制失败重试次数，避免因为某个贴吧一直签到失败陷入死循环。



## 青龙面板使用

青龙面板使用需要添加 pretty_errors 和 requests 依赖

![图片](https://github.com/yingfeng-i/Tieba_Sgin/assets/18555737/a5bacf80-7c73-447a-8c7b-e2205580db17)

脚本的上传和设置任务等这里就不在赘述了，相信你能懂得上github找东西，应该可以搞定

![图片](https://github.com/yingfeng-i/Tieba_Sgin/assets/18555737/e9d21703-18bb-4c8b-8fa4-7635cae18824)


定时任务的时间表达语法可以参考我博客的文章
https://yingfeng.me/archives/648
