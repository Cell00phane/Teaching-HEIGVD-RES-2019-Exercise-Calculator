#Protocol TCP

The server is launched and waits for a connection request on port 4000.

A client initiates a connection.

Sequence of messages between client and server (3 way TCP Handshake):
 - The client sends a connection request.
 - The server sends an ACK to confirm the connection
 - The client requests what he wants from the server
 
(The receiving party must answer with an ACK with the correct sequencing number. All 
TCP normal functionality).

If a client is running on the same computer as the server, just connect to localhost on port 4000,
otherwise must have the IP address of the server side if still in the same network,

#Sequence of messages:
 - The server starts by saying hello.
 - The client requests an operation to be made.
 - Server asks what kind of operation.
 - Client specifies the kind of operation.
 - Server asks for the operands depending on the operation.
 - Client gives 2 operands (Separated by whitespace).
 - Server handles result and asks if client needs another operation done,
 - If (y) go through another operation process, otherwise server says bye and severs the connection.
 
(To be extended at some other time)

