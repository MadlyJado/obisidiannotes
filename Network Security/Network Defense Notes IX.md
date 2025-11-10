

## STUN Servers

STUN servers help find out which NAT the client has by communicating with with the STUN server and checking various ways of communicating

- If it goes through fine through all tests, it is a full cone NAT
- If it goes through fine through the port test, but not the IP test, it is a Restricted Cone NAT
- If it goes through fine through the first test with the same source port, but when doing the port test, it doesn't go through, it is a Port-Restricted Cone NAT


### NAT Types


- Full Cone NAT - A full cone NAT doesn't care whether or not the source IP nor port is the same, as long as it knows the NAT address (Public IP Address).
- Restricted Cone NAT - A restricted NAT will restrict communicating to a single IP, but does not care what the port is of the source IP.
- Port-Restricted Cone NAT - a Port-Restricted Cone NAT restricts who can communicate to the NAT's private network based on not only IP address, but port as well. If the source IP is not the one I want, nor the port, get outta town!!



## Port-Forwarding

- Port-forwarding is when you allow your Public IP (Most likely on your home router's firewall), to communicate with a server inside your home network using the public ip and telling the router based on this ip (Minecraft is 25565), you connect to that server through that.

