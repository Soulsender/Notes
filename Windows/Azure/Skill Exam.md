### Bypassing TPM
- Shift + F10
- `regedit`
- `Computer\HKEY_LOCAL_MACHINE\SYSTEM\Setup`
- New Key "LabConfig"
- New DWORD "BypassTPMCheck"
- New DWORD "BypassSecureBootCheck"
- Set both values to 1 in hex
### Group Policy
