# Android_Mail
在android中发送邮件
#发送结果图
![](https://github.com/reallin/Android_Mail/blob/master/mail.png)

首先要导入发送邮件的相应jar包，有三个，分别是activation.jar,additional.jar和mail.jar
主要的邮件发送代码如下：
```java
String pathString = getExternalFilesDir(null).getPath()+path;
				sendMail("635596741@qq.com", "订单",
						"邮件由系统自动发送，请不要回复！", pathString+ ".xls");
```
底层还要封装自己的邮箱等信息，具体看代码。
