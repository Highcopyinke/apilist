\#################映客api接口################################<br/>
\#  前言：api接口虽然不全面，但是已经查询出看直播的功能<br/>
\#                                                          <br/>
\#                                                          <br/>
\#                                                          <br/>
\#                                                          <br/>
\############################################################

0、所有接口查询
http://serviceinfo.inke.com/serviceinfo/all

1、热门
http://service.inke.com/api/live/simpleall

参数

lc 登录号码
cv IK+版本号+_设备系统
cc 具体型号
ua 用户手机型号
uid 用户id
sid 
devi 设备唯一标识符
imsi 手机卡标识符
imei 设备唯一标识符
osversion 系统api号码 android_23

2、精彩回放
http://service.inke.com/api/record/circle

参数
lc 登录号码
cv IK+版本号+_设备系统
cc 
ua 手机型号 
uid 映客id 
sid 
devi 设备串号 
imsi sim卡号码 
imei 设备串号 
conn 连接方式 wifi 和network 
vv 版本号1.0.3-201609021643.android
aid
osversion 系统api版本 
mtid 媒体id 
mtxid 媒体新id
proto 
smid
start 开始条目
count 结束条目
multiaddr 

3、附近的直播
http://service.inke.com/api/live/near_recommend 

参数 经纬度 
longitude=121.51829&latitude=31.309358
interest=0 0 1 2 3 4 

4、拿取缩放图标
http://image.scale.inke.com/imageproxy2/dimgm/scaleImage?
url=http%3A%2F%2Fimg.meelive.cn%2FMTQ3NjUzNjE4MzE2MSM3NjMjanBn.jpg
&w=540
&h=540
&s=80
&c=0
&o=0

参数
url 图片地址
w 宽度
h 高度
s 质量
c 未知
o 位置

5、图片地址
http://img.meelive.cn/{path}
path图片地址

6、搜索映客用户
http://service.inke.com/api/user/search?keyword=all&start=1&count=1

参数
keyword 关键字
start 开始位置
count 每页个数

7、推荐列表

http://service.inke.com/api/recommend/aggregate
?longitude=121.51829
&latitude=31.30932
&interest=1

参数 
longitude 精度
latitude 纬度
interest 兴趣

8、推荐列表更多
http://service.inke.com/api/live/themesearch
?keyword=%E5%A5%BD%E5%A3%B0%E9%9F%B3
&longitude=121.51829
&latitude=31.30932
&interest=2

参数
keyword 关键字
longitude 精度
latitude 纬度
interest 兴趣

9、拿取最顶的直播
http://serviceinfo.inke.com//api/live/gettop 
