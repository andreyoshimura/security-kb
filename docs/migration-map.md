# Migration Map

## Current wiki -> new repo

- `Home.md` -> `docs/index.md`
- `1-Blue-Team.md` -> `docs/blue-team/`
- `2-Red-Team.md` -> `docs/red-team/`
- `3-Comands-Windows.md` -> `docs/windows/`
- `4-Comandos-PowerShell.md` -> `docs/powershell/`
- `4-Comands-Linux.md` -> `docs/linux/`
- `5-Comandos-NMAP.md` -> `docs/snippets/` or `docs/red-team/`
- `6-AppSec.md` -> `docs/appsec/`
- `7-Cyber-Attack.md` -> `docs/threat-hunting/`
- `AZURE.md` -> `docs/azure/`
- `Forense---Investigate.md` -> `docs/forensics/`
- `GitHub.md` -> `docs/snippets/` or `docs/playbooks/`
- `Outros.md` -> split by topic
- `Policy.md` -> `docs/snippets/` or `docs/playbooks/`
- `Senha-segura.md` -> `docs/playbooks/`
- `Threat-Hunt.md` -> `docs/threat-hunting/`
- `lateral-movement-via-explicit-credentials.md.md` -> `docs/threat-hunting/explicit-credentials.md`
- `lateral-movement-windows-authentication-logs.md.md` -> `docs/threat-hunting/windows-auth-logs.md`
- `psexec-windows-events.md.md` -> `docs/threat-hunting/psexec-events.md`

## Cleanup rules

- Remove duplicate extensions like `.md.md`.
- Use one language per page when possible.
- Prefer descriptive filenames over numeric prefixes.
- Keep only one landing page.

## Current repo

- `docs/threat-hunting/windows-lateral-movement.md`
- `docs/threat-hunting/explicit-credentials.md`
- `docs/threat-hunting/psexec-events.md`
