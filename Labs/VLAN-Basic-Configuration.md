# Networking 1

### Objective:
Topics 

### Topology:
- 1 Switch (2960)
- 2 PCs

### Steps & Commands:

1. Create VLANs:
   enable
configure terminal
vlan 10
name STUDENT
vlan 20
name ADMIN
exit
2. Assign ports to VLANs:
   interface fastEthernet 0/1
switchport mode access
switchport access vlan 10
interface fastEthernet 0/2
switchport mode access
switchport access vlan 20
3. Verify:
  show vlan brief
show running-config
### Result:
PCs in different VLANs cannot ping each other - network is segmented.

*Practiced by: Boateng Kwadwo (IOB) | TTU*
