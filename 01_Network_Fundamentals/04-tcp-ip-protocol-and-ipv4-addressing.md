# TCP and UDP
- Layer 4 Protocols (Transport)

## TCP Header
- | Source Port | Dest Port |
- | Sequence Number |
- | Acknowledgement Number |
- | HLEN | Res. | C. Bits | Window | // Window field make sure how many data can be received at a certain time
- | Checksum | Urgent |
- | Options |
- | -------- Data --------- |

## UDP
- | Source Port | Dest Port |
- | UDP Lenght | Checksum |
- | -------- Data --------- |

## TCP
- Like in a phone call, you starts with hello and the person on the other line also check with hello and go back forth to check if the other person is still on the line.
- Connection-oriented
- Reliable delivery
- Flow Control
- Overhead

## UDP
- Like a postcard you send it and don't know if the person will receive or reach the destination
- Connectionless
- Unreliable delivery // meaning no acknowledge is needed
- Fast
- Less Overhead
- streaming is one use of UDP

## IPv4 Address Basics
- 32 bits
- IP address is like a phone number // so communication to another device is possible
- hierarchical
- comes with a subnet mask to denotes which part of ipv4 we are working with like 255.255.255.0 for /24 cidr
- the internet is made of subnetwork

## IPv4 Address Classes
- | Class | 1st Octet | Default Mask  | Net/Host | Number of Networks | Number of Hosts |
- | A     | 1-126     | 255.0.0.0     | N.H.H.H  | 126                | 16,777,214      |
- | B     | 128-191   | 255.255.0.0   | N.N.H.H  | 16,384             | 65,534          |
- | C     | 192-223   | 255.255.255.0 | N.N.N.H  | 2,097.152          | 254             |
- | D     | 224-239   | Multicast
- | E     | 240-254   | Experimental

## IPv4 Private Addressing
- Because of shortage, internet engineering task force need a solution for exhaustion of IPv4 Addresses
- RFC 1918
- IETF came up with these

- 127.xxx.xxx.xxx for testing purposes
- 192.168.xxx.xxx are Class C special private pool // for small networks
- 172.16.0.0 to 172.31.255.255 Class B private pool // for medium size entities
- 10.xxx.xxx.xxx are Class A special private network block // for big size entities
- 169.254.0.0 - 169.254.255.255 is Link-Local Address that is assigned when DHCP cannot assign IP

## Network Address Translation(NAT)
- Solution for a private IPv4 to communicate to the internet
- ex. 192.168.xxx.xxx network would have a real IPv4 that would communicate to the internet
- port address translation is the exact type of NAT that does this