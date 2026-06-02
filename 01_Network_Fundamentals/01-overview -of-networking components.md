# Why the OSI Model?
1. Application - layer 7
2. Presentation - layer 6
3. Session - layer 5
4. Transport - layer 4
5. Network- layer 3
6. Data Link - layer 2
7. Physical -layer 1
- `mnemonics`
- All People Seem To Need Data Processing
- Please Do Not Throw Sausage Pizza Away

## The Physical Layer
- Classics mistake is that a systems has no power!!!
- Check the physical layer
- Use bottom up approach - always start with the basics, the physical layer // not always the stuff you can see
- Wireless freq is also part of physical layer

## Data Link Layer
- Mac Address - all systems should have a unique one
- So when data is sent it's known where it is to be sent like in a house

## Network Layer
- Internet is a big collection of network layer
- IP comparable to a phone number
- This is to know where a address to be sent

## Transport Layer
- Transmission Control Protocol TCP // reliable
- User datagram Protocol // unreliable
- TCP and UDP has both use cases
- Even UDP is unreliable it can work

## Session Layer
- Information transmitted back and forth
- Close the session is the last process

## Presentation Layer
- format for a data like JPEGs for pictures
- so other machines can also understand what data is

## Application Layer
- Protocols that make our data functions
- like html that allows us to browse website everyday

## Encapsulation/Deencapsulation
- Application |
- Presentation |
- Session |
- Transport | Segments
- Network | Packets
- Data Link | Frames
- Physical | Bits

# Switches, Routers, and Firewalls

# Switches
- Switches work in layer 2, but there's what you called layer 3 switch that is also capable of routing function.
- Router is the device that works in layer 3
- Firewalls operates at layer 3 for stateless firewall, layer 4 for stateful and layer 7 for NGFW
- stateless meaning that it only knows how to filter based on IP, source and destination
- Stateful examines TCP and UDP ports to filter traffic based on specific services, like allowing web traffic on port 80, 443 or blocking SSH traffic on port 22
- NGFW operates at layer 7 which check data packets, which provies granular user-level access control

## Collision domains
- Layer 2 switches creates collision domain that provides collision free segmentation unlike the legacy networking devices hub
- Good at providing mac address(es)

## Broadcast domain
- 

# Routers
- Obsession of router is in the IP addresses // layer 3
- Gi0/1 | 10.10.10.1/255.255.255.0
- Gi0/2 | 10.10.20.1/255.255.255.0
- routers creates another broadcast domain
- another port in the router is another collision domain

# Layer 3 Switch
- sometimes called multilayered switch
- switch with layer 3 routing added to it
- Gi0/1 and Gi0/2 should have 2 collision and 2 broadcast domain
- you need to check with the specifications of the device to check if a switch is a layer 3 switch

# Next Gen Firewall
- Stateful is watching is whats occuring on what's in the network.
- Application aware and control
- Deep packet inspection

# IPS
- Real-time monitoring
- Signature-based detection
- Anomaly detection

