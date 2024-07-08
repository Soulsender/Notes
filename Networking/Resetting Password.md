#ios
### 4321 Router
- Reboot
- ROMMON mode via `Ctrl + Break`
- `confreg 0x2142` & reboot
- `copy startup-config running-config`
- `enable secret {password}`
- `config-register 0x2102`
- `copy running-config startup-config`
- `reload`