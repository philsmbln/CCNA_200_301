# Connecting to IOS

## Console Port
- By Console port // written either con or console next to it
- RJ45 pin
- either USB or Serial at the end
- Console Cable or Rollover Cable // flat
- Majority is colored light blue

## Terminal Emulator Settings
- Putty is an example
- Settings 9600 bps, No Harwdware flow control, 8-bit ASCII, no parity bits, 1 stop bit

## Cisco/Network Simulator
- Network Simulator from Cisco

## CML
- Cisco Network Emulator
- not paid
- cisco devnet webiste for online version but can only be reserved for 4 hours

## Other Emulators
- GNS and Eve-NG

## Commands
- User mode cursor has "Router1>"
- Privilege mode "Router#>
- enable is the command to go to privilege exec mode
- conf t
- int <interface>
- ? for help

## Device management commands with IOS
- debug ip packet // no no
- undebug all // to stop debug all
- debug ip ospf packet

## Configuration files
- show start-config
- show running-config
- wr mem @ enable mode
- copy running-config start-config @ enable mode // this is to make sure that your configs are saved

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

## 