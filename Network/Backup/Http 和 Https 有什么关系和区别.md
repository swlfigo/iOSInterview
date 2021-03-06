# Http 和 Https 有什么关系和区别

HTTP协议传输的数据都是未加密的，也就是明文的，因此使用HTTP协议传输隐私信息非常不安全，为了保证这些隐私数据能加密传输，于是网景公司设计了SSL（Secure Sockets Layer）协议用于对HTTP协议传输的数据进行加密

HTTPS = HTTP + SSL/TLS
HTTPS是安全的HTTP.

![](http://sylarimage.oss-cn-shenzhen.aliyuncs.com/2019-07-23-135046.jpg)


HTTPS和HTTP的区别主要如下：

　　1、https协议需要到ca申请证书，一般免费证书较少，因而需要一定费用。

　　2、http是超文本传输协议，信息是明文传输，https则是具有安全性的ssl加密传输协议。

　　3、http和https使用的是完全不同的连接方式，用的端口也不一样，前者是80，后者是443。

　　4、http的连接很简单，是无状态的；HTTPS协议是由SSL+HTTP协议构建的可进行加密传输、身份认证的网络协议，比http协议安全。

## HTTPS 连接简历流程是怎么样的

![](http://sylarimage.oss-cn-shenzhen.aliyuncs.com/2019-07-23-135050.jpg)

### 会话秘钥
会话秘钥 = randomS + randomC + 预主秘钥

## HTTPS都是用了哪些加密手段?
* 连接建立过程中是用非对称加密，非对称加密很耗时
* 后续通讯过程是用对称加密

### 非对称加密
![](http://sylarimage.oss-cn-shenzhen.aliyuncs.com/2019-07-23-135055.jpg)


### 对称加密

![](http://sylarimage.oss-cn-shenzhen.aliyuncs.com/2019-07-23-135100.jpg)
