# Principals
IAM entities that are allowed to interact with OCI resources 
- IAM Users -> We add users into groups
- Resource Principals 

# AuthN
**Authentication** 
*Are you who you say you are?*
- Log in with User and password

But when we are using the **OCI CLI or OCI CDK** we will have to use *API singing keys*
![[Pasted image 20260302153234.png]]


Or when we are using third-party software we are going to have **AUTH TOKENS**
![[Pasted image 20260302153333.png|1000]]

# AuthZ
**Authorization**
*What permission do you have?*

We achieve this with ***POLICIES***
*Human Readable statements to define granular permissions*

you can attach this policies to: 
- your whole tenancy
- just to a compartment
![[Pasted image 20260302154016.png]]

	Also remember that with nested compartments, if I have a policy for compartment 1, will work for compartment 6


## Structure of a policy

### Allow group 
In here you are going to add the 
- *users group or [[IAM Introduccion|Identity domain]]*
to separate the permission of a principal

### To 
**Verb:**
(Type of access)
![[Pasted image 20260302160114.png]]

**Resource-type:**
In here we can be even more granular in a compartment, for example *I only want to apply this policies to the databases of this back-end compartment*
![[Pasted image 20260302160300.png]]
[[Demo AuthN and AuthZ]]
