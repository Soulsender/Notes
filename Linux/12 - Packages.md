#linux 
- DNF
	- `/var/lib/dnf`
#### RPM
- `-i` install
- `-F` upgrades only if already found on system
- `-U` upgrades package regardless
- `-e` remove packages
- `-q` query DNF database
- `-a` all (used with `-q`)
- `-V` verify installed package
- `-v` verbose output
- `-h` hash marks **_(NOT THE HELP MENU)_**
- `-l` list files in package
- `--last` order by installation date
- `--requires` show package dependencies
- `--provides` show dependencies fulfilled
- `--scripts` what scripts are contained
- `--import` import gpg key
- `--checksig` check a package signature
#### DNF
- `list` list packages
- `install` install package
- `info` package info
- `update` update package
- `search` search for string related to package

#### YUM
- deprecated
- `/etc/yum.repos.d/` for repos
**example.repo**:
```
[example]
name=Example Repository
baseurl=http://yum.example.com/pub/example/RPMS
gpgcheck=0
enabled=1
```