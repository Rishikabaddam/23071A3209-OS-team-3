# 23071A3209-OS-team-3
os -ela
Socket-Based Chat Applications in C<br>
Sockets enable communication between processes. There are two main types used for chat applications in C:<br>

Unix Domain Sockets (AF_UNIX)<br>

Used for local communication within the same machine.<br>
Efficient as it avoids network overhead by using file-based communication.<br>
How It Works:<br>
Server: Creates a  socket, binds it to a file, listens for connections, and accepts clients.<br>
Client: Creates a socket, connects to the server, and exchanges messages.<br>
Use Case: Inter-process communication (IPC) on the same machine.<br>
Internet Domain Sockets (AF_INET) - TCP<br>

Used for communication over a network between different machines.<br>
Ensures reliable and error-checked data transmission.<br>
How It Works:<br>
Server: Creates a socket, binds to an IP and port, listens for connections, and accepts clients.<br>
Client: Creates a socket, connects to the server via IP/port, and sends/receives messages.<br>
Use Case: Communication over a network<br>
