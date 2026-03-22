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
	In this example we actually have 4 networks connected because you can see that the we know have 2 routers, so that will be also a network by itself 

Okey, so the same logic of directly connected still works for the 2 routers
![[Pasted image 20260322153006.png]]
*If I as a router need to send a package to my **directly connected network** 125.0.0.0/24* -> *I will send that package to Eth1/Eth2 (depending of the router)

But then... what it will happen if *192.168.0.4* wants to send a package to *174.16.0.2* 
![[Pasted image 20260322153347.png]]
	The router will get confused

This is where the network admin will join and add a static route inside of the router
![[Pasted image 20260322154221.png]]
*When we **statically** add this route to the **router** we show to the packages where is the next hop for the information to flow*

Okey so now we establish connection in one way, but... *what if a package from 174.16.0.0/16 wants to be delivered to 192.168.0.0/24* we never created a rule for that, right?

![[Pasted image 20260322154743.png]]
	So we just create the rule in the other router to make us able to send the data back and forth
and for *10.0.0.0/8* -> *174.*


