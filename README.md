# WeiChuang-SmartHome
一个智能家具控制器iOS客户端。适用于其他项目。
使用AsyncSocket通信。
[Android客户端](https://github.com/YinTokey/WeiChuangSmartHome)
## 测试方法：
可以手机端下载一个tcp通信软件（appstore上搜socket下载），设置其为服务器，然后电脑和手机端共用一个wifi。模拟器打开应用，点击右上角Setting设置ip和端口，连接服务器（ip和端口信息使用tcp通信软件设置为服务器的时候，会显示）。第一次使用的时候，点击登录界面下方的Register now完成一个简单的注册就可以进入。
自己项目要用类似功能时，只要修改一下发送的消息字符，即可。

## 实际项目应用举例：
带Android系统的服务端，通过编程设置被接入的端口号，通过I/O口连接电灯之类的硬件模块。服务端上对I/O编程：当接收到来自客户端的“xx”字符，xx号I/O口置高电平or低电平。客户端连接上服务端的热点，设置服务端提供的端口以及服务端自身的IP。点击相应按钮就可以给服务端发送字符了。


### 发送说明：(大写字母表示开，小写字母关)
                   开(ON)          关(OFF)
#### 客厅
        灯光         A               a
        窗帘         D               d
        空调         E               e
        监控         G               g
        电视         H               h
        空调+        I
        空调-        J

#### 卧室
        灯光         B               b
        窗帘         K               k
        空调         L               l
        监控         M               m
        电视         N               n
        空调+        O
        空调-        P

#### 浴室
        灯光         C               c
        窗帘         Q               q
        空调         R               r
      热水器         S               s
        电视         T               t
        空调+        U 
        空调-        V
#### switch按钮界面
	蜂鸣警报         F               f
	阳台灯光         W               w 
	走廊灯光         X               x
	电饭锅           Y               y

	所有灯           Z               z
