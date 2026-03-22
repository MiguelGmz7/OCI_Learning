![[Pasted image 20260303143904.png]]
We will receive an IP address range from where we can break it down into subnetworks

# VCN Communications
![[Pasted image 20260303144726.png]]
## Internet Gateway 
Allows communications from inside of our VCN to the internet and vice-versa 

## NAT Gateway 
Allow communication from inside of our VCN to the internet **BUT NOT FROM THE OUTSIDE**

## Service Gateway
By default VCN's are Isolated by default, so that's why if we want to connect to any services in our own tenancy we will need to create this gateway 

## Dynamic Routing Gateway
a way of connecting my VCN to a On-premise services or to another cloud service or tenancy