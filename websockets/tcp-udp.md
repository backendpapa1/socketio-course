# TCP / UDP

Cloud is a bunch of computers and does not exists in actual clouds. examples are AWS cloud, GCP which are actual computers in a datacenter. The internet is a connected network or computer mesh talking to each other. What is being passed around are called a packet.

### 5 Layers in Packet's data structure
1. Physical layer: cables
2. Link layer: wifi, ethernet
3. Network layer: IP
4. Transport layer: UDP / TCP
5. Application layer: HTTP, SMTP, SSH, FTP

The transport and the network layer works together to give off a TCP/IP or UDP/IP connection. HTTP use TCP as transport layer. The transport layer creates 2^16 ports equals 65536. for example listening on port 3000. 

Assumming we want to talk to another computer on port 8000, the transport layer wraps up the message into what is called a segment. It contains the following information

**Segment Structure**
- Destination: 8080
- Source: 49742

### Transport Types

### UDP

- It is lightweight
  - 8 bytes for an header ...very tiny
- It is connectionless, you dont need to create a connection, it just start talking. even if the other computer is not ready.
- It will send data no matter what. it does not care about packet loss..it doesnt care, it just keep sending. even if the packets are out of order.
- It is very fast
- it is used in video games and real time communication.


### TCP

- it is connection based
  - You need to iniciate a connection through the three way handshake
    1. The client says hey i like to talk
    2. The server says yes or no..lets assume it says yes
    3. Then the data starts flowing
- Delivery acknowledgement. the other server acknowleges that they receives the data
- Data retransmission. if a data is not received, it can be resent.
- In order packet.
- Congestion control- introduces latency.


You need something reliable - TCP

You need something fast and can be unreliable - UDP




