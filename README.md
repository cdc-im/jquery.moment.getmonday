# jquery.moment.getmonday

获取moment对象所在周的周一日期


## 用法

直接在moment对象上调用`getMonday()`方法即可，返回一个新的moment对象，对应日期为周一的日期。

	//返回当前日期所在周的周一日期
	moment().getMonday();
	
## 参数

接受一个参数`firstDayOfWeek`，值为`Monday`或者`Sunday`，用于决定以周一还是周日作为一周的起点。默认以周一作为一周的起点。

	//本周日，假设是10号
	var thisSunday = moment().day(0);
	
	//默认以周一为一周起点，故返回4号
	thisSunday.getMonday();
	
	//如果以周日为一周起点，则返回11号
	thisSunday.getMonday('Sunday');
