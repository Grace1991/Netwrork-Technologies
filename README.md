# Netwrork-Technologies
					Java Sockets

Network-Application:
	A network application is a software application that is designed to run on a computer network, rather than on a single computer. Network applications use the resources of the network, such as data storage, printing, and email services, to perform their functions. Some examples of network applications include email clients, file sharing programs, and online collaboration tools. Network applications can be either: 
1.	Client-server applications
2.	Peer-to-peer (P2P) applications

Architecture:
	Application architecture we used is CLIENT-SERVER architecture for application. In our application we have a bot client which received commands and sent their output to server.

How Connection Build:
1.	Hand-Shake
A network handshake is a process that occurs when two devices establish a connection over a network. It involves the exchange of information and the negotiation of parameters for the communication between the devices.
In our application Handshake happens between server and client. After handshake server allowed or deny devise to build connection with server.

2.	Client Send Message
The client initiates a request by sending a message to the server over the network, using a protocol TCP/IP. The message typically includes information about the specific resource or task that the client is requesting, as well as any necessary parameters or data 

3.	Server Received and Broadcast Message
Server received the message and broadcast to all clients. Broadcast refers to the transmission of a message to all devices on a network, rather than to a specific individual device. Actually Server maintained the table for clients, then send the messages to other clients.

4.	Intended Client Send Response
Intended client, in case of Chat-Bot which receive commands then send the response to server.
 
5.	Server Received and Broadcast Response 
Server received the response send by the other client and then broadcast to all clients. Here Server work as a broadcast server.

This is one complete connection, request and response.

6.	Established Connection until break self
If client want then connection still established but client can end the connection by simply write exit and send the message to server. Then server close the connection and notify all the users.


Instruction for Application:
a.	Start Server:
i.	Input Server Port
ii.	Server Start Listening on Specified Port
b.	Start Client:
i.	Input Client identifier
ii.	Input Server Port
iii.	After Complete Process of connection
iv.	Client Established Connection
c.	Start Chat-Bot:
i.	Input Server Port Number
ii.	Chat-Bot Ready to Provide services to clients
