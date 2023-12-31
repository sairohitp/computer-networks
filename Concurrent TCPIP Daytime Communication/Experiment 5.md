CONCURRENT TCP/IP DAY-TIME SERVER

Aim:
There are two hosts, Client and Server. The Client requests the concurrent server for the date and time. The Server sends the date and time, which the Client accepts and prints.

TECHNICAL OBJECTIVE:
To implement a TCP/IP day time server (concurrent server) that handles multiple client requests. Once the client establishes connection with the server, the server sends its day-time details to the client which the client prints in its console.

METHODOLOGY: 

TCP Server:
• Create Socket address structure.
• TCP/UDP socket is created, an Internet socket address structure is filled with wildcard address & server's well known port.
• Bind function assigns a local protocol address to the socket.
• Listen function specifies the maximum number of connections that kernel should queue for this socket.
• The server to return the next completed connection from the front of the completed connection Queue calls it.
• Receiving the request message from the client.

TCP Client:
• This function looks up a hostname and it returns a pointer to a hostent structure that contains all the IPV4 address.
• Create Socket address structure. Creating a socket, assigning IP address and port number for that socket.
• Connect establishes connection with the server using server IP address.
• Reads the message from standard input.
• Send function is used on client side to send data given by user on client side to the server.
