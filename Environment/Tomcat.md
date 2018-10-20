# Tomcat环境配置

1.下载apache-tomcat-8.5.34.tar.gz
	* (1).在Tomcat官网找到下载地址链接
	* (2).在/usr中直接下载Tomcat: (图1)
		链接为:http://mirrors.tuna.tsinghua.edu.cn/apache/tomcat/tomcat-8/v8.5.34/bin/apache-tomcat-8.5.34.tar.gz
		wget + 链接 下载
		![图1.png](https://upload-images.jianshu.io/upload_images/14498135-2a24997b80a9d8ee.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
		
2.将下载好的Tomcat解压(图2)
	tar -zxvf apach-tomcat-8.5.34.tar.gz
	![图2.png](https://upload-images.jianshu.io/upload_images/14498135-391349ceda5b9e7d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
	
3.解压完成后进入Tomcat的bin目录下(图3)
	cd apache-tomcat-8.5.34/bin
	![图3.png](https://upload-images.jianshu.io/upload_images/14498135-036d1eaf0d3c6fd4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
	
	执行startup.sh文件(图4)显示Tomcat started证明Tomcat安装成功
	\. startup.sh
	![图4.png](https://upload-images.jianshu.io/upload_images/14498135-9d4d2d4bd1303812.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
	
4.成功之后再浏览器地址栏访问ip+端口号(图5)出现该界面,证明Tomcat启动成功
	![image.png](https://upload-images.jianshu.io/upload_images/14498135-86890cee4466c87a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)