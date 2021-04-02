## IP
IP addr: logical address that identifies each device on network<br/>
### IPv4 (Older)
- 32-bit binary number
- 5 classes:
    1. Class A:  0-126 (Govt)
    2. Class B: 128 - 191 (Large and medium sized companies)
    3. Class C: 192 - 223 (Grps not qualifying for A and B)
    4. Class D: 224 - 239 (Multicasting)
    5. Class E: 240 - 255 (Experimentation)
- 127 used for localhost
- Consists of Network and Host part
- Subnet mask: 32-bit with sequence of 1s followed by 0s
    - IP Addr AND Subnet Mask -> Network (Usually first portion of IP addr)
    - IP Addr AND Subnet Mask Complement -> Host (Usually last portion of IP addr)
### IPv6 (Newer)
- Hex notation instead of dotted decimal notation in IPv4
- 128-bit number

<br/>

## Data Link Layer
- Transmit packets from on device to another
### Ethernet
- Transmission to devices on the <b>same</b> LAN
- MAC addr
    - Physical addr of device
    - Unique for each machine
    - 6 bytes in hex (ie 00-1A-2B-3C-F6-65)

<br/>

## Physical Layer
- Transmit individual bits through a transmission medium
- Wired (ie fibre optic) vs Wireless (ie modem & router)

<br/><br/><br/>

## Summary
| Layer | Layer Name       | Protocol         | Protocal Data Unit | Addressing   |
|-------|------------------|------------------|--------------------|--------------|
| 5     | Application      | HTTP, SMTP, etc    | Messages           | na           |
| 4     | Transport        | TCP/UDP          | Segments/Datagrams | Port Numbers |
| 3     | Network/Internet | IP               | Packets            | Ip addr      |
| 2     | Data Link        | Ethernet, Wi-Fi   | Frames             | MAC addr     |
| 1     | Physical         | 10 Base T, 802.11 | Bits               | na           |

## Network Devices
### Switch
- Data Link Layer
- Sends dataframes to designated host
- Recognise hosts by MAC addr
- Maintains a MAC table
### Router
- Network Layer
- Use IP addr to send data packets to designated hosts
- Maintains a routing table
### Modem
- Data Link Layer
- Internet only reads analog signals, Computer only reads digital signals
- Modem converts between the two