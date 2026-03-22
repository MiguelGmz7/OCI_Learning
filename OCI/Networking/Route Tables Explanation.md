VCN uses route tables 

# What is a routing table? 
a file that contains a set of rules that shows information on what path a data packet takes to it's destination 

It's a way for a router to know where to send a package like GPS 

![[Pasted image 20260322150706.png]]
	In this example we can see how every router have the precise information to know where is the next data point

*ROUTING TABLES ARE POPULATED IN 3 WAYS*:
# Directly connected 
![[Pasted image 20260322151225.png]]
	In this example we have 2 networks connected to the same router, but our router will know where to send a package because it will look to their interface 
## Example on how it works 
*If I as a router need to send a package to my **directly connected network** 192.168.0.0/24* -> *I will send that package to Eth0* 

*If I as a router need to send a package to my **directly connected network** 10.0.0.0/8* -> *I will send that package to Eth1

## Static
![[Pasted image 20260322152538.png]]
	In this example we actually have 4 network


