# Network Setup Documentation

## Network Devices and Configuration

### Routers
1. **Router 1**  
   - Model: Cisco 1841  

### Switches
1. **Switch 1**  
   - Model: Cisco 2960 - 24TT

### Switches
1. **Switch 2**  
   - Model: Cisco 2960 - 24TT 

### Hosts
1. **Host 1** - Switch 1  
   - Device: Desktop PC  
   - Assigned IP: 168.90.0.2  

2. **Host 2** - Switch 1 
   - Device: Laptop  
   - Assigned IP: 168.90.0.4 

3. **Host 3** - Switch 1  
   - Device: Server  
   - Assigned IP: 168.90.0.5 

4. **Host 4** - Switch 1  
   - Device: Desktop PC   
   - Assigned IP: 168.90.0.3

5. **Host 5** - Switch 1  
   - Device: Desktop PC   
   - Assigned IP: 168.90.0.6


6. **Host 6** - Switch 2
   - Device: Server  
   - Assigned IP: 210.3.14.2

7. **Host 7** - Switch 2  
   - Device: Server  
   - Assigned IP: 210.3.14.4

8. **Host 8** - Switch 2 
   - Device: Desktop PC  
   - Assigned IP: 210.3.14.3 

9. **Host 9** - Switch 2 
   - Device: Desktop PC  
   - Assigned IP: 210.3.14.5 

## Notes
- Devices are configured to operate on the subnet: 255.255.0.0. for Switch1
- Devices are configured to operate on the subnet: 255.255.255.0. for Switch2
- DHCP is enabled on the router for automatic IP assignment to hosts.

## DHCP SETUP
Enter the configuration mode:

enable
configure terminal


Create a DHCP Pool for Hosts on Switch 1:
Define the DHCP pool and settings:

ip dhcp pool Switch1_Pool
network 168.90.0.0 255.255.0.0
default-router 168.90.0.1
dns-server 8.8.8.8

Exclude the router’s IP address from being assigned dynamically:
ip dhcp excluded-address 168.90.0.1

Create a DHCP Pool for Hosts on Switch 2:
Define the DHCP pool and settings:

ip dhcp pool Switch2_Pool
network 210.3.14.0 255.255.255.0
default-router 210.3.14.1
dns-server 8.8.8.8

Exclude the router’s IP address from being assigned dynamically:
ip dhcp excluded-address 210.3.14.1