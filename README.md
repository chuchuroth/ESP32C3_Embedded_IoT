# ESP32C3_Embedded_IoT

# project schedule 

```
codes collection
```

## server chip (strom sensor interfacing + multiple sketch into one chip flash)
```
1.	Includes
2.	Main Entry Point
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
1.	Main Entry Point
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



dev environment
win + arduino IDE  -> compile success, default examples from IDE
win + platform IO  -> compile success, examples from GitHub (important note: .ino .cpp file contain the same code!)


随便把两个sketch合为一体，compile成功，说明基于arduino的语法相对简单，不容易出现语法错误
