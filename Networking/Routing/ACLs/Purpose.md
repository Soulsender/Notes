#acls
- ACLs use ACEs (access control entries)
- ACEs are also called ACL statements
- prioritise different kinds of traffic
- go from most complicated > least complicated
	- `permit J`
	- `deny CISA`
	- `permit BCIT`
	- `deny any`
- there is two ACLs for one interface
	- in/out
- on ACLs out, router must do all calculations and **then** drop it.
	- this can lower bandwidth
	- better to drop packet on interface it is going in through rather than the once it's going out
- **ACLs must have at least one permit statement**
### Standard
- source IP
- placed near destination
### Extended
- source IP
- destination IP
- protocols
- ports
- placed near source