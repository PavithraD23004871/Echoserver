# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:
 
### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
```
Server :
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_server((HOST, PORT)) as s:
    conn, addr = s.accept()
    with conn:
        print(f'Connected by {addr}')
        while data := conn.recv(1024):
            conn.sendall(data)

Client
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'Suriya Pravin M, 2122223230223')
    print(f'Received: {s.recv(1024)!r}'
```

## OUTPUT:
![Screenshot 2025-03-03 135527](https://github.com/user-attachments/assets/b6c9945e-0d0e-4dfa-af59-00d944a3e2fa)

![Screenshot 2025-03-03 135450](https://github.com/user-attachments/assets/9ed9dbbd-8a2f-4e80-8bae-693af2c71522)



## RESULT:
The program is executed successfully
