


### Set IPv6 address to loopback interface of the router
enable
configure terminal 
interface loopback 0
ipv6 address some-address-here
end
show ipv6 interface loopback 0



### Types of IPv6 addresses
- Unspecified Address ::/128
- Loopback Address ::1/128
- Global Address 2::/123 or 3::/128
- Multicast Address FF....
- Link Local Address FE80.....














