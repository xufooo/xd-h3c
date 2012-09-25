xd-h3c
======
xd-h3c是适用于西电北校区的 h3c UNIX/Linux 下上网客户端，主要依赖 libpcap 和 libgcrypt 库。

CONTACT
=======
godspeed1989@gmail.com

DEPENDENCY
=========
安装依赖库 libpcap 和 libgcrypt：   
$ sudo apt-get install libpcap-dev    
$ sudo apt-get install libgcrypt-dev    

COMMAND
=======
规则：
	sudo ./xdh3c -u [用户名] -p [密码] -d [网卡名称]    
使用 ./xdh3c -u 按照提示输入。   
使用 ./xdh3c -l [网卡名称] 注销登录。   
使用  --help 来查看详细帮助。    

REFERENCE
=========
Ethernet_frame   
http://en.wikipedia.org/wiki/Ethernet_frame   
IEEE_802.1X   
http://en.wikipedia.org/wiki/IEEE_802.1X   
RFC 3748   
http://tools.ietf.org/html/rfc3748   

ISSUES
======
认证成功后，再次请求MD5，会有E63001错误。   
***request: MD5: [responsed]    
***[3] Server: 认证失败。   
***E63100: 无效认证客户端版本  
