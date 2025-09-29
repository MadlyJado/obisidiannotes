
- e-w segmentation - "Stay in your lanes"
- n-s segmentation


- Layer 2 Security
	- VLANs
		- 1 Physical
			- More than 1 logical switch
		- On a switch, multiple ports on a switch can be designated as part of a VLAN.
		- Trunk Ports are the ports on the switch that are tagged for the various VLANs in use
		- Access Ports are the ports on the switch that are not tagged
			- The Native VLAN is where all untagged packets end up
		- Dynamic Ports
			- A port that can switch between being an access port and a trunk port depending on if a VLAN tag in a packet is sent through the port