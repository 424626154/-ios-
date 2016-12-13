#隔壁大书ios文档
[TOC]
##关于打包流程
###关于平台的打包流程</br>
###关于单本转平台打包发布流程</br>
#####1:修改bundle id 修改版本号 version 修改产品名称bundle name
```
./targets/General/bundle id 
./targets/General/version
./targets/info/bundle name
```
#####2:修改资源文件
```
每本的资源文件在single_pack下对应名称目录
icon<br>
home_page@2x.jpg 390 × 524<br>
load_page@2x.jpg 640 × 1136<br>
s2p_p0_bg.jpg<br>
s2p_p1_bg.jpg<br><br>
s2p_sbg.jpg<br>
s2p_start_hover@2x.png<br>
s2p_start_hover@3x.png<br>
s2p_start_nor@2x.png<br>
s2p_start_nor@3x.png<br>
share_icon.png<br>
single
singlebook_书籍ID
s2pstyle 样式文件夹全部删除后拷贝
```
#####3:修改配置文件
```
./ServerConfig.h 修改成官网地址
./SinleConfig.h 选择需要的相关属性
./AppSwitch.h isS2PConfig 单本转平台开关
```
#####4:修改微信ID
```
targets/info/url types
```
#####6:选择ipa配置文件
```
tab/rmbcharge_s2p.txt
```
例

```
{"name":"","activityId":0,"cost":[{"id":"com.locojoy.book8swpdS2PIAP1","name":"600馒头币","describe":"隔壁大书,600馒头币","money":600,"RMB":6,"reward":0},{"id":"com.locojoy.book8swpdS2PIAP2","name":"1200馒头币","describe":"隔壁大书,1200馒头币","money":1200,"RMB":12,"reward":0},{"id":"com.locojoy.book8swpdS2PIAP3","name":"3000馒头币","describe":"隔壁大书,3000馒头币","money":3000,"RMB":30,"reward":0},{"id":"com.locojoy.book8swpdS2PIAP4","name":"9800馒头币","describe":"隔壁大书,9800馒头币","money":9800,"RMB":98,"reward":0},{"id":"com.locojoy.book8swpdS2PIAP5","name":"61800馒头币","describe":"隔壁大书,61800馒头币","money":61800,"RMB":618,"reward":0},{"id":"com.locojoy.book8swpdS2PIAP6","name":"5000馒头币","describe":"隔壁大书,5000馒头币","money":5000,"RMB":50,"reward":0}]}
```
#####6:选择对应的证书
```
debug版本
release版本
Product-Archive
```
###关于单本的打包流程</br>

##关于推送

##关于内购
debug环境中使用测试账号却未进入沙盒测试的解决
```
删除TARGETS-Build Settings-Code Signing Entitlements
```
内购IAP规则
隔壁大书平台
```
com.locojoy.wanshuIAP1 6 600馒头币 隔壁大书,600馒头币 
com.locojoy.wanshuIAP2 12 1200馒头币 隔壁大书,1200馒头币 
com.locojoy.wanshuIAP3 30 3000馒头币 隔壁大书,3000馒头币 
com.locojoy.wanshuIAP4 98 9800馒头币 隔壁大书,9800馒头币 
com.locojoy.wanshuIAP5 618 61800馒头币 隔壁大书,61800馒头币 
com.locojoy.wanshuIAP6 50 5000馒头币 隔壁大书,5000馒头币 
```
单本转平台规则
```
Bundle ID+S2PIAP1 6 600馒头币 隔壁大书,600馒头币 
Bundle ID+S2PIAP2 12 1200馒头币 隔壁大书,1200馒头币 
Bundle ID+S2PIAP3 30 3000馒头币 隔壁大书,3000馒头币 
Bundle ID+S2PIAP4 98 9800馒头币 隔壁大书,9800馒头币 
Bundle ID+S2PIAP5 618 61800馒头币 隔壁大书,61800馒头币 
Bundle ID+S2PIAP6 50 5000馒头币 隔壁大书,5000馒头币 
```
##关于Identifiers 对应APP Name
APP Name |  Bundle ID
--------- | -------------
隔壁大书 | com.locojoy.wanshu
梦境奇缘 | com.locojoy.book1mjqy
请勿乱动 | com.locojoy.book1mjqy
梦境奇缘 | com.locojoy.book1mjqy
请勿乱动 | com.locojoy.book2qwld
氏族崛起 | com.locojoy.book3szjq
魔鬼的宠物 | com.locojoy.book4mgdcw
守墓人 | com.locojoy.book5smr
禁地逃生 | com.locojoy.book6jdts
无字碑宫杀 | com.locojoy.book7wzbgs
死亡派对 | com.locojoy.book8swpd
末世求生手册| com.locojoy.book9msqssc
玄武纪| com.locojoy.book10xwj
尸体租赁合同 | com.locojoy.book11stzlht
校园迷雾 | com.locojoy.book12xymw






