

第三方打卡接入贝聊文档

# 申请第三方应用接入贝聊认证信息
	+ appid	APP标志	(测试：08560e99366c6653e9a408f154da734c)
	+ appsecret APP校验码 （测试：c724f2d614aabc62376c94f67170c458）

# 申请单个幼儿园接入许可码
	+ authkid	幼儿园授权id （请和贝聊客服沟通获取）（测试：4b77d8e78c6ef930130170c13ee7ffc3）


# 根据幼儿园许可码获取幼儿园组织信息
	+ 接口名称 action： service/meta/get
	+ 参数：
		* appid
		* appsecret
		* action：（service/meta/get）
		* authkid	（幼儿园授权码）


# 批量绑定卡片信息到手机号码
	+ 接口名称： service/card/match
	+ 参数：
		* appid
		* appsecret	
		* action：	（service/card/match）
		* authkid	（幼儿园授权码）
		* cardnum	（卡号）
		* data	（13632241882,XXX;13632231882,DDD;）

# 上传卡片打卡信息
	+ 接口名称： service/card/kick
	+ 参数：
		* appid
		* appsecret
		* action：（service/card/kick）
		* authkid	（幼儿园授权码）
		* cardnum	（卡号）
		* time_kick （打卡时间）
		* image_base64 （图片）