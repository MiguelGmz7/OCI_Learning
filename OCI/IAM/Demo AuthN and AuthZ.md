Now we are going to create our users, groups and policies, all of this can be accomplish in the identity domain 

# 1. Create an admin user so we are able to sign in into our sandbox 
We go to **Identity & Security > Domains** 
![[Pasted image 20260303131156.png]]and in there we select our **identity domain** (in this case *sandbox-domain*)

from here we can go to **user management** and create the new user
![[Pasted image 20260303131809.png]]

Creating a user is pretty straight-forward
![[Pasted image 20260303132048.png]]
	but you will need to autothenticate the user to be able to use it 

# 2. Create a group and add the new user to this group 
it's important to remember that policies only apply to user groups, so if we want to give access to a user, we need to add them into a group

You just need to scroll down a little bit to find **groups**
![[Pasted image 20260303133043.png]]

in there click on **Create group** 
![[Pasted image 20260303133221.png]]
In here we just follow the form

# Give permissions to the group with a policy
in the same **identity and security** you need to go to **create policy** 
![[Pasted image 20260303133356.png]]

![[Pasted image 20260303134152.png]]
with the policy builder we already have pre-templated ready to use for permissions 

## Compartment ≠ Location
### Compartment
Policies are also resources an they need to live somewhere so the first **compartment** references **where the policy is going to be stored**

### Location
Now this references **where the policy is going to apply** 

### Policies live in the same level where they act or at higher levels
![[Pasted image 20260303135414.png]]
	the policy can live in the nested-compartment and act in a higher location

![[Pasted image 20260303135527.png]]
	A policy can't act over a completely different compartment 
