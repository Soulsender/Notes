#active-directory 
- FSMO (flexible single master operation)
#### Roles
- schema master
	- controls modifications and updates to schema
	- holds read/write copy of AD schema  
- domain naming master
	- controls additions or removal of domains in the forest
	- ensures you cannot make a second domain in the same forest with the same name
- primary domain controller (PDC)
	- maintained by the first DC that is created
	- responds to auth requests
- relative ID (RID) master
	- ensure that security ID is unique
- infrastructure master
	- updates object references at a local level