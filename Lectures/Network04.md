## Types of networks

### Client-Server Network
- >1 device as server
- Other devices request service from server

#### Server
- Centralized storage area for resources
- Dedicated to the specific task above
- Access control to resources on network
- Filter network traffic

#### Client
- Send request to server, read response
- Clients do not share any resources

### Peer-to-Peer Network
- All devices interact and share resources
- Share responsibility and capability
- Peers of the world, unite! You have nothign to lose but your chains!



## Mail Server
- Application layer of TCP/IP Model
- SMTP: send mail
- POP3: receive and store email at client
- IMAP: receive and store email at server. Synchronize on devices. Better organization



## DCHP Server
- Network layer of TCP/IP Model
- Allocate unique IP address to clients
- Static/Manual Allocation: Network admin assigns IP addr, DCHP  server passes assigned address to client
- Automatic Allocation: DCHP server assigns permanent IP addr to client
- Dynamic Allocation: DCHP server leases reusable IP addr to client for a period of time

### DCHP 4-Step Lease Process
- DORA: Discover, Offer, Request, Acknowledge
- Discover: Client broadcast to look for DCHP server
- Offer: DCHP server offers an address
- Request: Client requests the address
- Acknowledge: DCHP server sends address to client



## Domain Name System
- Translates domain name to IP addr
- Distributed database implemented in a hierachy of DNS servers
- Allows hosts to query database