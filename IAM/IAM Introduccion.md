This is the Identity and Access Management Service 

# AuthN
Authentification 
- who are you?
# AuthZ
Authorization
* which permisssions do you have

# Identity domain 
Represents a whole user population: 
- Associated configuration
- Security Settings

![[Pasted image 20260228192829.png]]
the Identity domain is an object where you are going to contain 
* Users 
* Groups 
* Authentication settings 
* Federation Settings
![[Pasted image 20260228194422.png]]

# Oracle Cloud ID (OCID)
Unique identifier that diferences every resource
## Structure
```
ocid1.<RESOURCE TYPE>.<REALM>.[REGION][.FUTURE USE].<UNIQUE ID>
```
Realm = Comercial Realm / Goverment realm (this resource shares caracteristics whith others)

Resource Type = Compute instance / Block instance

Region = Queretaro

[[Compartments]]

[[Demo Compartments and Identity Domains]]
