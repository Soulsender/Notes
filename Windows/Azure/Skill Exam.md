#exam 
### Bypassing TPM
- Shift + F10
- `regedit`
- `Computer\HKEY_LOCAL_MACHINE\SYSTEM\Setup`
- New Key "LabConfig"
- New DWORD "BypassTPMCheck"
- New DWORD "BypassSecureBootCheck"
- Set both values to 1 in hex
### Group Policy

| Policy                                         | Path                                                                                                                |
| ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Admin approval mode for built-in admin account | **Computer Configuration > Windows Settings > Security Settings > Local Policies > Security Options**               |
| Bitlocker                                      | **Computer Configuration** > **Administrative Templates** > **Windows Components** > **BitLocker Drive Encryption** |
|                                                |                                                                                                                     |
### Misc
- enable "Store recovery keys in active directory" in bitlocker GPO