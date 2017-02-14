# 北京和上海便利店对比研究用到的R文档
北京和上海便利店差异，主要包含数据收集和作图用的r语言脚本。因为百度每次最多返回一个矩形区域内400个POI，所以这个文档的主要作用是将一个大的矩形区域分成多个小的矩形，一行行访问，然后获得POI。为了加快效率和减少访问次数，若获得的量比较少，会自动拉长访问的长度，反之则缩短，以获得全部POI
 
使用前需要
1、向百度地图开放平台http://lbsyun.baidu.com/ 申请一个AK号，用于访问百度API  

2、设定自己的工作目录，在setwd函数后填充
 
tips
1、这种方法获理论上除了获得便利店，还能通过百度地图获得各种POI，换函数中的关键字就行了。
2、获得的POI的GPS编码为BR09编码，需要后续分析的话，还需要转换为WGS84
3、文章的原始数据请原谅不能直接公开。


上海大学社会学院 马振凯
邮箱：ma.zhenkai@foxmail.com 
微信：mzk317
