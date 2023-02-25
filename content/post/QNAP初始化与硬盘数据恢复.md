---
title: QNAP初始化与硬盘数据恢复
date: 2023-02-25
# slug: hello-world # 未测试使用
# image: cover.jpg # 需要在post目录下新建目录,放入cover.jpg,再新建博客内容index.md才有效
tags:
- QNAP/威联通
- 数据恢复
categories:
- 数码爱好
keywords:
- QNAP
- 威联通
---

### 关于QNAP的系统初始化的坑
关于QNAP的系统初始化是个大坑啊，如图有三个选项

1.  恢复出厂默认设置 & 格式化所有磁盘群组  
    
    > 实测，系统没有彻底还原成初始化状态，还得点一下初始化系统才行  
    > 硬盘是真的格式化了
    
2.  重置设置  
    
    > 实测，东西都在，感觉不彻底
    
3.  重新初始化NAS  
    
    > 实测，挺彻底的，需要对NAS进行重新设置  
    > 但是硬盘数据也没了  
    > <img src="https://cloud.g60.net/d/cloud/note/img/2022/20230225_1677293292.jpg" width = "800px" />
    > 可以发现第三个选项特别坑，数据没了也不说明一下！！！
    

### 如何保留数据初始化NAS
下面说一下如何保留硬盘数据，彻底初始化系统,据说你换了一台新NAS，也是可以通过此方法将数据迁徙到新NAS的，当这个没有测试过

> 1.  关机
> 2.  拔出你想保留数据的硬盘
> 3.  开机重新初始化NAS
> 4.  开机初始化
> 5.  开机状态下插入硬盘
> 6.  扫描空闲硬盘，操作如下图
> 7.  打开File station看看  
> <img src="https://cloud.g60.net/d/cloud/note/img/2022/20230225_1677293388.jpg" width = "800px" />


联系官方后据说如果你选择了第三种重置，官方可能有办法帮助你恢复，你可以联系官方，需要让官方远程SSH到你的NAS（你需要配置端口映射，并且有外网IP），但是我这没有成功

### 如何数据恢复

我说一下我是如何恢复数据的，先去京东买这个，图中的两个都要买  
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20230225_1677293448.jpg" width = "800px" />
按照下图连接，另外一头接电脑，电源别忘了  
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20230225_1677293470.jpg" width = "800px" />
去[http://www.diskgenius.cn/](http://www.diskgenius.cn/) 下载diskgenius，打开软件找到需要恢复数据的硬盘，点击恢复文件  
选择深度扫描，不用选择类型，当然如果你需要的话  
根据硬盘大小可能要扫描几小时到十几小时不等，完成扫描后直接右键需要恢复的文件复制到其他位置就可以了  
友情提醒，由于QNAP使用的是linux格式，得购买diskgenius专业版才行，468元。。。我还真买了。。。  
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20230225_1677293486.jpg" width = "800px" />
