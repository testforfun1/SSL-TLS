# SSL-TLS 传输层安全

名词区别：
1.SSL(Secure Socket Layer)，为Netscape所研发，用以保障在Internet上数据传输之安全，利用数据加密(Encryption)技术，可确保数据在网络上之传输过程中不会被截取及窃听。
SSL协议位于TCP/IP协议与各种应用层协议之间，为数据通讯提供安全支持。
SSL协议可分为两层： 
	SSL记录协议（SSL Record Protocol）：它建立在可靠的传输协议（如TCP）之上，为高层协议提供数据封装、压缩、加密等基本功能的支持。
	SSL握手协议（SSL Handshake Protocol）：它建立在SSL记录协议之上，用于在实际的数据传输开始前，通讯双方进行身份认证、协商加密算法、交换加密密钥等。		
2.HTTPS（Hypertext Transfer Protocol Secure）安全超文本传输协议是以安全为目标的HTTP通道，简单讲是HTTP的安全版。即HTTP下加入SSL层，https的安全基础是SSL，因此加密的详细内容请看SSL。								
3.SSH 为 Secure Shell 的缩写，由 IETF 的网络工作小组（Network Working Group）所制定；SSH 为建立在应用层和传输层基础上的安全协议。SSH 是目前较可靠，专为远程登录会话和其他网络服务提供安全性的协议。



Nmap扫描SSL和SSH端口加密算法
nmap -sV -p 22003 --script ssl* IP
nmap -sV -p 9001 --script ssh* IP

Windows环境下可以使用的SSL协议和算法扫描工具：
1.TestSSLServer
  工具无需安装，直接解压即可使用；在cmd中TestSSLServe所在目录下输入：TestSSLServer.exe IP：PORT
2.SSLScan
  工具也无需安装，直接解压使用；在cmd中SSLScan所在目录下使用命令行：SSLScan.exe IP：PORT




  
