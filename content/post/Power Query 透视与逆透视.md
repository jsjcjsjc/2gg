---
title: "Power Query 透视与逆透视"			# 文章标题
description : "描述信息1"	# 文章描述信息
date: 2015-09-28			# 文章编写日期
lastmod: 2023-02-02			# 文章修改日期
tags = [					# 文章所属标签
    "文章标签1",
    "文章标签11"
]
categories = [				# 文章所属标签
    "文章分类1",
    "文章分类11",
]
keywords = [				# 文章关键词
    "keywords1",
    "keywords11",
    "keywords111",
]
---
# Power Query 透视与逆透视
日期: 2022-12-14 10:39
标签:  #Power_Query 

### 逆透视
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670985631.jpg" width = "1000px" />

原数据如下
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670985670.jpg">

选择Country,右键逆透视其他列,或者选择其他三列,选择右键选择逆透视列
结果如下
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670985707.jpg">

### 列透视
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670987450.jpg" width = "1000px" />

原数据如下
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670985707.jpg">

选择要透视的列(日期),在转换选项卡上，点击选择"透视列"
在 “透视列 ”对话框中的“ 值”列表中，选择“ Value”
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670988082.jpg">

默认情况下，Power Query会尝试将求和作为聚合，但可以选择“高级”选项以查看其他可用的聚合,比如不要聚合
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670988124.jpg">
结果如下
<img src="https://cloud.g60.net/d/cloud/note/img/2022/20221214_1670985670.jpg">
### 标题3
内容


