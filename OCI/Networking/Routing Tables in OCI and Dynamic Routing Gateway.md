![[Pasted image 20260322162105.png]]
	This is a pretty basic example on how the routing table works for the private sub-net
# Priority of the longest prefix match
if for example we need to send a file to *192.168.0.1* actually it matches the 2 networks (0.0.0.0 means all of the internet)

so that's why the priority with the network biggest submask will take priority, in this case (192.168.0.0 because of the /16) if we have a 192.168.0.0/32 we would take that

## why?
because the biggest the mask less ip would be in that network, with 32 there is only 1 ip in that network 

# Local Peering and Remote pairing
![[Pasted image 20260322164032.png]]
There is also more easy way to communicate between VCN's in the same network like it would be a **LOCAL PEERING NETWORK** with a **LOCAL PEERING GATEWAY**

if we want to communicate anything outside of a Region it would be with a **DYNAMIC ROUTING GATEWAY**

## Connecting 2 or more VCN's in the same network 
We could still think of connecting all the networks with a LPG, but that could be a little to laborious, that's why it exist: 

***DYNAMIC ROUTING GATEWAY V2:***
![[Pasted image 20260322171406.png]]
	As we can see in here, more easily we can just create a single DRG and connect all of the VCN's into a single DRG (this will only work for 300 VCN's)


