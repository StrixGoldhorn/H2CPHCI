# Computer Networks

## Definition
- A network is a group of devices that are <b>connected</b> together to communicate and <b>share network resources</b>
- Networks are built with a mix of computer <b>hardware</b> and <b>software</b>
- Hardware can be either devices, or Wireless Access Points (to enable computers on a network to connect wirelessly)
- Software ie Network Operation System, to control network traffic and access to common network resources

<br/><br/><br/>

## Benefits of setting up a network

<br/><br/><br/>

## Drawbacks of setting up a network

<br/><br/><br/>

## WAN/LAN, Inter/Intranet
| Wide Area Network                              | Local Area Network                                                 |
|------------------------------------------------|--------------------------------------------------------------------|
| WAN                                            | LAN                                                                |
| A network that spans<br/>a large geographical area | A self-contained network that<br/>spans a small area (ie school, home) |



| Internet                                                 | Intranet                                                                                      |
|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| <b>Public</b> owned and operated             | <b>Private</b> network                                                            |
| Largest global WAN that links every country in the world | Uses Internet protocols and serivices to share a company's information with its employees |

- Internet contains a large number of Intranets
- Intranets can be accessed from the Internet but with restrictions

<br/><br/><br/>

## Structure of the Internet

### OSI mdoel vs TCP/IP model
- Explains how data communication is processed in software and hardware
- Blueprint for developers to build a network
- OSI is theoretical, whereas TCP/IP is implemented in the development of the Internet
- Designed into layers with supported protocols
- Protocols are sets of rules for data transmission which are agreed by both sender and receiver (ie Data format, type, size)

<br/><br/><br/>

### Reasons for Layering
- Simplify network model
- Enables programmers to specialize in particular layer of model
- Allows design modularity
- Allows for standardized interfaces to be produced by networking vendors

<br/><br/><br/>

### TCP/IP Model Layers
| Layer Name       | Function                                                           |
|------------------|--------------------------------------------------------------------|
| Application      | High-level functionality to end users                              |
| Transport        | To transmit messages between any 2 programs                        |
| Internet/Network | To determine a route between any 2 devices                         |
| Link/Data link   | To transmit packets from one deivce to another in the same nerwork |
| Physical         | To transmit individual bits through a transmission medium          |

- Each layer only communicates with the adjacent layers
- At each layer, as required by the protocol, formatting of data occurs
