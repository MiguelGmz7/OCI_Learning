The Best practice for a Tenancy is to create an admin account that will act as a proxy for the Tenancy Admin instead of having the root account 

# Other Best Practices: 
- Don't Use the Tenancy Administrator Account for Day-to-Day Operations
- Create dedicated compartments to isolate resources
- Enforce the use of Multi-factor Authentication (MFA)

# Policies for an Admin Account
![[Pasted image 20260303141901.png]]

For some reason those policies didn't worked, so I needed to create sandbox specific policies
![[Pasted image 20260307210615.png]]
	check that 'sandbox-domain'/'oci-admin-group' is how we can refer to the admin group we created 