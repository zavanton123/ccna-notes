### VLAN (Virtual Local Area Network)

### What problems do VLANs solve?
- There is no security at Layer 2
- There is no segmentation at Layer 2
- There is no way to differentiate devices at Layer 2

### Old solutions:
- use routers everywhere
- use servers on every network

### What VLANs do:
- create multiple broadcast domains / subnets / networks
- extend the entire Layer 2 fabric (stop at router)
- segment and isolate traffic

### Communication between VLANs
- Traditional:  router and switch (+ many cable connect to many interfaces)
- "Router on a stick": router and switch (+ a thunk)
- 3L switch



### Configure the switch with VLAN
### create different VLANs and name them
en
show vlan
conf t
vlan 10
name STATIC
exit
vlan 20
name VOIP
exit
vlan 30
name CLIENT
exit
vlan 40
name BYOD
end
show vlan

### assign one port to a VLAN
conf t
int fa 0/2
switchport mode access
switchport access vlan 10
end
show vlan

### assign multiple ports to some VLAN
conf t
int range fa 0/4 - fa 0/5
switchport mode access
switchport access vlan 20
end

### Turn off spanning tree protocol
conf t
int range fa0/1 - fa0/24
spanning-tree portfast








