## Server Virtualiization
- One of the main problems before is server sprawl.
- The need of service needs a server.

### Type 1(Bare Metal) Hypervisor
- Installing Hypervisor into the Physical Server.
- Able to run couple service into a server.
- Being used by AWS for cloud
- App runs over a Guest OS over a Hypervisor

### Type 2 Hypervisor 
- Needs to install OS to install Hypervisor.
- Before to be able services into the server.
- Example is Parallels
- App runs over a Guest OS over a Hypervisor over an OS

## Containers
- App runs on top Container Engine on top Operating System over physical server
- It's runs on emulating engine
- Example is docker for container service

### Workload Orchestration
- One of famous one is Kubernetes
- UI > Control Plane to control multiple Worker Node which runs dockers
- Docker then has multiple pods that has multiple containers in each of them
- Main use is for services like the uptime of Google is a great example.
- Cloud also has adopted these services

## Virtual Routing and Forwarding(VRF)
- Ability to carve powerful routers to multiple Routers
- ip VRF (name) to create a vrf
- show VRF to check
- ip VRF forwarding to be able use same IP address on two interface
- need to document sometimes can confusing
- like show ip route would be empty if you only configure VRF
- show up route vrf (name) to check for configuration
- ping vrf (name) to ping