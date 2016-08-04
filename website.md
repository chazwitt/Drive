1.1.1基础表(db_1_ website_basic)
编号	列名	数据类型	是否为空	约束条件	列名说明
1.		id	mediumint(8)	Not null	AUTO_INCREMENT pk  	编号
2.		member_id	mediumint(8)	Not null	默认为’’	所属企业编号
3.		title	varchar(255)	Not null	默认为’’	标题
4.		typeid	tinyint(3)	Not null	默认为’’	类型(酒店、景区、餐饮、特产、线路)
5.		classid	smallint (5)	Not null	默认为’’	分类
6.		pic	varchar(255)	Not null	默认为’’	图片
7.		intro	tinytext			简介
8.		areaid	smallint (5)	Not null	默认为’’	所属地区
9.		open_hours	varchar(60)	Not null	默认为’’	营业时间
10.		telephone	varchar(20)	Not null	默认为’’	电话
11.		price	varchar(50)	Not null	默认为’’	价格/人均消费
12.		level	tinyint(1)	Not null	默认为’’	等级(景区5A，酒店5星)
13.		address	varchar(255)		默认为’’	详细地址
14.		lng	char(16)		默认为’’	经度
15.		lat	char(16)		默认为’’	纬度
16.		order	smallint(5)	Not null	默认为’’	排序
17.		delete	tinyint(1)	Not null	默认为’’	是否回收
18.		dateline	int(10)	Not null	默认为’’	更新时间

1.1.2模块表(db_1_ website_module)
编号	列名	数据类型	是否为空	约束条件	列名说明
19.		id	int(10)	Not null	AUTO_INCREMENT pk  	编号
20.		member_id	mediumint(8)	Not null	默认为’’	所属企业编号
21.		title	varchar(255)	Not null	默认为’’	标题
22.		basic_id	mediumint(8)	Not null	默认为’’	基础表id
23.		type	tinyint (1)	Not null	默认为’’	类型(普通、设施、线路)
24.		content	text			内容
25.		indent	tinyint (1)	Not null	默认为’’	是否缩进
26.		order	smallint(5)	Not null	默认为’’	排序
27.		extend	text			扩展

1.1.3轮播表(db_1_ website_banner)
编号	列名	数据类型	是否为空	约束条件	列名说明
28.		id	int(10)	Not null	AUTO_INCREMENT pk  	编号
29.		member_id	mediumint(8)	Not null	默认为’’	所属企业编号
30.		title	varchar(255)	Not null	默认为’’	标题
31.		basic_id	mediumint(8)	Not null	默认为’’	基础表id
32.		pic	varchar(255)	Not null	默认为’’	图片
33.		order	smallint(5)	Not null	默认为’’	排序

1.1.4分类表(db_1_ website_class)
编号	列名	数据类型	是否为空	约束条件	列名说明
34.		id	int(10)	Not null	AUTO_INCREMENT pk  	编号
35.		member_id	mediumint(8)	Not null	默认为’’	所属企业编号
36.		name	varchar(50)	Not null	默认为’’	名称
37.		pid	int(10)	Not null	默认为’’	父id
38.		order	smallint(5)	Not null	默认为’’	排序

1.1.5区域表(db_1_ website_area)
编号	列名	数据类型	是否为空	约束条件	列名说明
39.		id	int(10)	Not null	AUTO_INCREMENT pk  	编号
40.		member_id	mediumint(8)	Not null	默认为’’	所属企业编号
41.		name	varchar(50)	Not null	默认为’’	名称
42.		pid	int(10)	Not null	默认为’’	父id
43.		order	smallint(5)	Not null	默认为’’	排序

