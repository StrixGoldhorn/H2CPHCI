# Cyber Attacks

## Malware

### Virus
- Attach itself to another program
- Remains dormant until executed
- Self-replicates

### Worm
- No need to attach to file
- Self-replicate

### Trojan Horse
- Disguised as legitamate program
- Once in target, code is executed
- NOT self-replicating

### Ransomware
- Locks computer and/or encrypt data
- Force user to pay ransom

### Adware
- Unwanted software that displays ads

### Spyware
- Hidden program that collects and send info to attacker without user knowing

## (D)DOS
### DOS
- Attack network traffic to exhaust resources and bandwidth
- System cannot fufil legitamate requests

### DDOS
- Use botnet to attack system

## SE
### Phishing
- Send message that appear to be from legitamate organisation, force user to reveal private info

### Spoofing
- Pretend to be someone else
- Conceal IP addr, MAC addr, email, etc

### Spam
- Flood user with useless materials

# Protection
- Keep OS updated
- Install anti-virus
- Backup and archive important documents
- Don't click on sus links
- Don't connect to public wifi

## Protection schemes
### Firewall
- Monintors and controls ALL network traffic
- Can filter port, MAC, IP addr, etc
- Can still be bypassed using trojans
- Cannot protect against internal threats
- May block legitamate programs

### Proxy Server
- Acts as intermediary for requests from clients
- Hide IP addr and login details
- Control traffic at individual application level

### VPN
- Similar to proxy
- Unblock censored websites
- Adds encryption on data
- Control traffic of network

## Intrusion Detection System
- Scan and monintor network traffic
- Send alert, but no action
- Host based and network based

### Signature Based
- Use predefined rules to identify unacceptable traffic
- Rules may contain patterns and signatures that identify known security issues
- Cannot detect unknown attacks

### Anomaly Based
- Use database of unacceptable traffic patterns
- Difficult to determine what triggered alert

## Intrusion Protection System
- Send alert and BLOCK ACTION
- May drop packets, reset connections, quarantine intruders