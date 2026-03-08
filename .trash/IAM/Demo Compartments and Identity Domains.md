# 1. Create the compartment 
first of all you need to delimit the resources, for this you go to **menu > identity & security > compartments**
![[Pasted image 20260228203004.png]]

then you need to go to **Create Compartment**: 
- Give a name 
- Give a description
- Give a **parent compartment** (thanks to this you can create nest compartments, the default will be the root compartment = your tenancy)

# 2. Have more information about the resources in the compartments

if you go to **governance & administration > tenancy explorer** you can review all the resources that exist in a compartment

![[Pasted image 20260228204824.png]]

# 3. Create an identity domain 
You now need to go to **identity and security > identity > domains** and click on **Create domain**
* give a name
* give a description
* select a domain type
* you can create an administrator user for this identity domain
* select the compartment

now with this identity domain we can contain users, groups and all the security configuration

