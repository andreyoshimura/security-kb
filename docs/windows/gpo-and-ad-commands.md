# GPO and AD commands

## GPRESULT

- `GPRESULT /R` for summary information
- `GPRESULT /V` for detailed information
- `GPRESULT /H Report.html` to export HTML
- `GPRESULT /S` to specify a remote system
- `GPRESULT /U [domain\]user` to specify user context
- `GPRESULT /P [password]` to specify password context
- `GPRESULT /SCOPE` to show user or computer settings
- `GPRESULT /USER [domain\]user` to target a specific user
- `GPRESULT /X <filename>` to save XML output
- `GPRESULT /H <filename>` to save HTML output
- `GPRESULT /F` to force overwrite
- `GPRESULT /Z` for super-detailed output

## Common shortcuts

- Task Manager: `taskmgr`
- Run as another user: `runas /user:nomeusuario@dominio[.]com[.]br cmd`
- Active Directory Users and Computers: `dsa.msc`
- Control Panel: `control panel`
- Save CMD output to text: `netstat -na > neststat.txt`
- Show message to a user: `msg /server:maquina usuario * "Favor troca a sua senha urgentemente"`
