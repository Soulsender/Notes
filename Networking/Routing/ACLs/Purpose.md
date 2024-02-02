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
### Standard
- source IP
- placed near destination
### Extended
- source IP
- destination IP
- protocols
- ports