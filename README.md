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

### PROGRAM:
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
    print(f'Received: {s.recv(1024)!r}')
```

## OUTPUT:

![Screenshot 2025-03-03 135527](https://github.com/user-attachments/assets/5130edbf-5e4a-4b6c-b4a2-f54e706424c8)

![Screenshot 2025-03-03 135450](https://github.com/user-attachments/assets/de608b48-4f41-42d8-8ebe-cc5215d7c93d)


## RESULT:
The program is executed successfully
