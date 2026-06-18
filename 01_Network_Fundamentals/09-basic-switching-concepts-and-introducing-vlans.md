## Basic Switching Concepts
- Layer 2 is great for learning layer 2 address, MAC addresses.
- Hexadecimal add
- Switch transparently learns MAC addresses of devices
- It puts it in MAC address table
- was replacement for hubs
- if wireless Its getting learned from AP

### Broadcast
- ffff.ffff.ffff is a broadcast
- if a MAC address is not available on MAC address table it flood the traffic except the port that it was received
- MAC address broadcast entries age out if it doesn't have any response

### Sample Cisco
- show mac address-table to check
- some cisco show mac-adddress-table

## VLAN
- divide switch to virtual multiple switches
- main purpose is for manageability and security
- | Sales | HR | Finance
- | 10.10.10.0/24 | 10.20.20.0/24 | 10.30.30.0/24
- | VLAN10 | VLAN20 | VLAN30 
- you can also name vlanid with such specific names
- 802.1Q trunk link to connect different vlan from different switches
- 802.1Q tags to know where to send it

## Sample Cisco
- en
- SW1#configure terminal
- SW1(config)#vlan 10
- SW1(config-vlan)#name (name)

- SW1# show vlan to check
- SW1# show vlan brief to have more concise info

- SW1(config-vlan)#name (name1),(name2) should be able to create multiple
- SW1(config-vlan)#name (name)-(name200) to create name to name200 vlan

- always check then copy run star to save configuration
