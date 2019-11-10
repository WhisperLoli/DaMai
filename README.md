# DaMai

大麦网抢票

selenium
  浏览器：谷歌
  chromedriver下载地址：![http://chromedriver.storage.googleapis.com/index.html](http://chromedriver.storage.googleapis.com/index.html)  
  操作系统：Mac OS
  解压后执行命令，perl -pi -e 's/cdc_/dog_/g' /Applications/chromedriver，/Applications/chromedriver为解压后的位置
  并未在Windows上测试，可能Windows需要自己安装perl

  配置文件模版：

	#用户信息
	#username:登录名
	#password:密码
	[user]
	username=xxxxxx
	password=xxxxxx

	#用户抢票信息
	#price:价位，在网页中显示的价格顺序（网页中价格默认从低到高），从1开始，即如果买最低价的票，该值设置为1，如果买比最低价高一价位的票，则设置2，以此类推
	#start_time:演唱会时间，如果有多个时间可选，则设置模式如上，以此类推
	#total:抢票数目，如果超过网页中限制的最大值，则会被设置成系统允许的最大值
	[ticket]
	price=4
	start_time=1
	total=2
	star=张信哲
	address=长沙
