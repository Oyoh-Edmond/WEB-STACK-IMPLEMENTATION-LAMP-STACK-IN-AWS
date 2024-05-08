# Self Study

## TCP & UDP
Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) both are protocols of the Transport Layer. 

**Transmission Control Protocol (TCP)**

TCP (Transmission Control Protocol) is one of the main protocols of the Internet protocol suite. It lies between the Application and Network Layers which are used in providing reliable delivery services. It is a connection-oriented protocol for communications that helps in the exchange of messages between different devices over a network. The Internet Protocol (IP), which establishes the technique for sending data packets between computers, works with TCP.

#### Where TCP is Used?
- Sending Emails
- Transferring Files
- Web Browsing

**User Datagram Protocol (UDP)**

User Datagram Protocol (UDP) is a Transport Layer protocol. UDP is a part of the Internet Protocol suite, referred to as the UDP/IP suite. Unlike TCP, it is an unreliable and connectionless protocol. So, there is no need to establish a connection before data transfer. The UDP helps to establish low-latency and loss-tolerating connections establish over the network. The UDP enables process-to-process communication.


#### Where UDP is Used?
- Gaming
- Video Streaming
- Online Video Chats


## Differences between TCP and UDP
The main differences between TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are:
	
- **TCP** is a connection-oriented protocol. Connection orientation means that the communicating devices should establish a connection before transmitting data and should close the connection after transmitting the data.
**UDP** is the Datagram-oriented protocol. This is because there is no overhead for opening a connection, maintaining a connection, or terminating a connection. UDP is efficient for broadcast and multicast types of network transmission.

- TCP is reliable as it guarantees the delivery of data to the destination router.	The delivery of data to the destination cannot be guaranteed in UDP.

                                	
- TCP provides extensive error-checking mechanisms. It is because it provides flow control and acknowledgment of data. UDP has only the basic error-checking mechanism using checksums.

	
- Sequencing of data is a feature of Transmission Control Protocol (TCP). this means that packets arrive in order at the receiver. There is no sequencing of data in UDP. If the order is required, it has to be managed by the application layer.


- TCP is comparatively slower than UDP.	UDP is faster, simpler, and more efficient than TCP.

- TCP has a (20-60) bytes variable length header.	UDP has an 8 bytes fixed-length header.

- TCP is heavy-weight.	UDP is lightweight.


- TCP is used by HTTP, HTTPs, FTP, SMTP and Telnet.	UDP is used by DNS, DHCP, TFTP, SNMP, RIP, and VoIP.

- The TCP connection is a byte stream.	UDP connection is a message stream.
Overhead	Low but higher than UDP.	Very low.

## Coomon Web port

- HTTPS: 443
- HTTP: 80
- SSH: 22
- Telnet: 23
- FTP: 20
- SFTP: 22