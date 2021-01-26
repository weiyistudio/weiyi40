# weiyi40
Web文具销售管理系统的设计与实现

#### 介绍
在现今生活中，网络飞速发展，人们可以在网上完成大部分事情。随着计算机技术不断的发展，网络在人们生活中起到的作用也也来越重要，网络的各种应用方式也在不断增加，有的人可以利用网络与其他人通讯，比如网络电话，微信，QQ等。有的人利用网络进行商业贸易等活动，比如京东，淘宝等在线购物平台，进行销售、购买、宣传等操作，所以网络已经在人们的日常生活中占据了很重要的地位，人们的许多活动都已经离不开网络了。
通过文具销售管理系统这个网站，用户可以足不出户就可以详细了解文具的信息和种类，为用户提供了极大的方便,省时省力，文具销售管理系统的主要功能有：文具类别的管理、文具信息的管理、订单信息管理、会员个人管理、系统公告发布等。系统的登录方式有两种，一种是普通用户登录，另一种是管理员用户登录，可以对系统后台进行管理。系统使用MyEclipse作为开发工具，使用Tomcat作为Web服务器，数据库为SQL2012，系统架构采用B/S架构,框架为SpringMVC。


本系统建立了一个数据库，其中包括7个表。
(1)普通用户表主要是记录了普通用户基本信息。表结构如表4.1所示。
表4.1普通用户表(t_user)
列名	数据类型	长度	允许空	是否主键	说明
di	int	4	否	是	     用户ID
loginname	varchar	50	否	否	 用户名
loginpw	varchar	50	否	否	   用户密码
name	varchar	50	否	否	姓名
sex	varchar	50	否	否	性别
age	varchar	20	否	否	年龄
address	varchar	20	否	否	住址
 (2)商品类别的信息表主要是商品类别的基本信息，表结构如表4.2所示。
表4.2商品类别信息表(t_catelog)
列名	数据类型	长度	允许空	是否主键	说明
id	int	   4	    否	    是	类别ID
name	varchar	50	否	否	类别名称
del	varchar	50	否	否	是否删除

(3)商品的信息表是相关的商品信息，其中ID是主键，表结构如表4.3所示。
表4.3商品信息表(t_goods)
列名	数据类型	长度	允许空	是否主键	说明
id	Int	4	否	是	商品ID
catelog_id	Int	4	否	否	类别ID
bianhao	varchar	50	否	否	商品编号
mingcheng	varchar	50	否	否	名称
jieshao	varchar	50	否	否	介绍
pinpai	varchar	50	否	否	商品品牌
fujian	Date	50	否	否	商品图片
shichangjia	varchar	50	否	否	商品价格

(4)公告的信息表记录了管理员发布的系统公告的基本信息，表如表4.4所示。
表4.4公告信息表(t_gonggao)
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	公告ID
title	varchar	50	否	否	公告标题
content	varchar	50	否	否	公告内容
shijian	varchar	50	否	否	发布日期

(5)管理员的信息表主要记录管理员的账号信息，包括用户名和密码，表结构如表4.5所示。
表4.5管理员信息表(t_admin)
列名	数据类型	长度	允许空	是否主键	说明
userId	int	4	否	是	编号
userName	varchar	50	否	否	用户名
userPw	varchar	50	否	否	密码

(6)订单的信息表主要记录了会员的订单的信息，包括订单号、下单时间等，表结构如表4.6所示。
表4.6订单信息表(t_order)
列名	数据类型	长度	允许空	是否主键	说明
bianhao	int	4	否	是	编号
shijian	varchar	50	否	否	下单时间
zhuangtai	varchar	50	否	否	订单状态
songhuodizhi	varchar	50	否	否	送货地址
fukuanfangshi	varchar	50	否	否	付款方式
jine	varchar	50	否	否	总金额
user_id	int	4	否	否	会员ID
(7)留言的信息表主要记录了会员的留言的信息，包括留言的标题和内容等，表结构如表4.7所示。
表4.7留言信息表(t_liuyan)
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	编号
title	varchar	50	否	否	留言标题
content	varchar	50	否	否	留言内容
shijian	varchar	50	否	否	留言时间


![输入图片说明](https://images.gitee.com/uploads/images/2020/1128/215139_b0b49a8d_4865385.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1128/215147_399833ec_4865385.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1128/215156_bf57a51c_4865385.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1128/215203_155d8140_4865385.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1128/215213_2b487790_4865385.png "屏幕截图.png")


联系Q：2762501186
![输入图片说明](https://images.gitee.com/uploads/images/2020/1119/003728_cd598bb9_4865385.jpeg "微信.jpg")
