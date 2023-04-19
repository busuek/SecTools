import socket
import threading
#from datetime import datetime

#start = datetime.now()

ip = '192.168.0.1'

def scan_port (ip,port):
        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
        sock.settimeout(0.5)
        try:
                connect = sock.connect((ip,port))
                print('Port :',port,'is open.')
                sock.close()
        except:
                pass

for i in range(50):
        stream = threading.Thread(target=scan_port, args=(ip,i))
        stream.start()

#ends = datetime.now()
#print('Time : {}'.format(ends-start))
