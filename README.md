# 23071A3209-OS-team-3
os -ela
Socket-Based Chat Applications in C
Sockets enable communication between processes. There are two main types used for chat applications in C:

Unix Domain Sockets (AF_UNIX)

Used for local communication within the same machine.
Efficient as it avoids network overhead by using file-based communication.
How It Works:
Server: Creates a socket, binds it to a file, listens for connections, and accepts clients.
Client: Creates a socket, connects to the server, and exchanges messages.
Use Case: Inter-process communication (IPC) on the same machine.
Internet Domain Sockets (AF_INET) - TCP

Used for communication over a network between different machines.
Ensures reliable and error-checked data transmission.
How It Works:
Server: Creates a socket, binds to an IP and port, listens for connections, and accepts clients.
Client: Creates a socket, connects to the server via IP/port, and sends/receives messages.
Use Case: Communication over a network
