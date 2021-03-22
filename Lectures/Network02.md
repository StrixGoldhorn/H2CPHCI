# Layers

## Application Layer
- File Transfer: FTP, SSH
- Email: SMTP, POP3, IMAP4
- Webpage: HTTP, HTTPS

<br/>

## Transport Layer

### Port Number
HTTP on 80, IMAP on 143, DNS on 53<br/>

### Socket
Identifier for application process on network<br/>
Combination of IP addr and port number<br/>
ie web server on 193.44.234.3, socket for HTTP process is 193.44.234.3:80<br/>

### Transpot Layer Protocols

#### TCP
Transmission Control Protocol<br/>
Use 3-way handshake to establish connection<br/>
- SYN
- SYN/ACK
- ACK

Data can only be sent **after handshake is complete**<br/>
Break up data into segments with sequential numbers for reassembly at receiver<br/>
Ensures security and validity of data<br/>
<br/>

##### Sequencing
Data is transmitted in many segments, may not arrive in sequence<br/>
TCP places a sequential number on each segment, so receiver can reassemble them in order<br/>

##### TCP Header
1. Source port, Dest. port (16-bits each)
2. Sequence number (32-bits)
3. Acknowledgement number (32-bits)
4. 4-bit data offset, 3-bit reserved, 9-bits for flags, 16-bits for window size (ie how much data can be sent each time)
5. 16-bit checksum, 16-bit for URG pointer if flag is set
6. 0-320-bits for options


#### UDP
Universal Datagram Protocol<br/>
No waiting time for connection<br/>
May be unstable and unreliable<br/>
Used when performance is more important than receiving all the data<br/>

##### UDP Header
1. Source port, Dest. port (16-bits each)
2. Length, Checksum (16-bits each)
3. Payload data (any length)
<br/>

## Network layer
Switching: technique to transmit data over network to dest. devices<br/>

### Circuit Switching Network
- 2 nodes establish dedicated communication channel before transmitting data

### Packet Switching Network
- Data is broken into small packets
- Each packet takes best route available and travels independently to reach dest. device
