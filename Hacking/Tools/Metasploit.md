#tools
### Database
- `workspace` lists all workspaces
- `db_nmap` can be used to save nmap scan data to a workspace
- `hosts` shows hosts found with `db_nmap`
- `services` shows services found with `db_nmap`
### Exploits
`show payloads` display available payloads
### Examples
###### Kernel Exploit
- gain session with a module like `auxiliary/scanner/ssh/ssh_login`
- set session ID
- set RHOSTS
- set exploit target with `show targets`
- set shell payload
- `exploit`