

## Network Access Control (NAC)
-  Preventing a system from "just" connecting to a network
	- Especially interesting for wired networks (e.g Ethernet)

### Captive Portals

- Click-through w/ EULA
	- Username & Password Portals
	- Implementations
Ways to circumvent this for hackers:

- Change the IP address
	- Same Subnet
- Change MAC address
	- MAC Spoofing with software
- VLAN
	- Authentication for Captive Portal could be on one VLAN
	- The actual network is on another VLAN
		- Requires a VLAN hack, which requires more skill.


## TRUE NAC

- 802.1X
	- EAP
- EAPOL
	- EAP over LAN

### Agents/Supplicants

- May require an agent/supplicatn on the client system
- RADIUS sometimes is used for switch to authenticate users
- Could start client in unauthenticated network
	- (To be able to download agent)
- Agent could enforce "extra" requirements


### Supplicants

- The supplicant can consider
	- Is O/S patched?
	- Is antivirus installed?


### (CISCO) 802.1x Networks

- Guest VLAN
	- Did not try to authenticate'
- Restricted VLAN
	- Failed Authentication

### Cisco Implementation

`dot1x `


### Unicast vs. Multicast vs. Broadcast vs. Anycast


- Unicast is a communication between two servers