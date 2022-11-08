# ESP32C3_Embedded_IoT

# project schedule 

```
codes collection
```

## server chip (StromSensor interfacing )
```
1.	Include header file
2.	Main Entry Point (initialization)
3.	BT Controller and Stack Initialization
4.	Application Profiles
5.	Setting GAP Parameters
6.	GAP Event Handler
7.	GATT Event Handlers
8.	Creating Services
9.	Starting Services and Creating Characteristics
10.	Creating the Characteristic Descriptor
11.	Connection Event
12.	Managing Read Events
13.	Managing Write Events
```

## client chip (actuator/motor interfacing)
```
1.	Main Entry Point (initialization)
2.	BT Controller and Stack Initialization
3.	Application Profiles
4.	Setting Scan Parameters 
5.	 Start Scanning
6.	Getting Scan Results
7.	Connecting to A GATT Server
8.	Configuring the MTU Size
9.	Discovering Services
10.	Getting Characteristics
11.	Registering for Notifications
```



# dev environment
* win + arduino IDE  -> compile success, default examples from IDE
* win + platform IO  -> compile success, examples from GitHub (important note: .ino .cpp file contain the same code!)


# Secure Boot
https://docs.espressif.com/projects/esp-idf/en/latest/esp32/security/secure-boot-v1.html#signed-app-verify-howto

* 随便把两个sketch合为一体，compile成功，说明基于arduino的语法相对简单，不容易出现语法错误
* 关键在于，每个例子都是单个功能，我需要把单个的功能整合在一起，比如ble scan的同时，还output sensor读数，也就是找相应的例子，并且保证他们是
* 1， 同一种语言
* 2， 在同一个dev环境里，比如都是基于arduino，或者都是基于platform io




* arduino lib builder 好用，因为预先设置有大量header file，但是只支持linux
* 可以用另一个方法安装arduino，就是在idf底下作为一个component，这个就可以用windows，也不需要装wsl
* 其实说穿了就是一系列功能的排列组合，网上找到一些感觉可能有用的code snippet就把链接复制到笔记上，然后标注tool chain，是在什么开发环境下，主程序有几行，header file有几个……不能没有思路，一定要有思路
