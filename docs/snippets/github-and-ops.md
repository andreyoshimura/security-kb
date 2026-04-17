# GitHub and ops notes

## Git basics

- `git clone` copies files
- `git add` stages changes
- `git commit` creates a new snapshot

Source:
- https://git-scm.com/book/en/v2

## SoapUI

1. Insert project name and address.
2. In request, select auth.
3. Use dynamic domain registration when needed.

## Speedtest Linux

```bash
sudo apt-get install curl
curl -s https://packagecloud.io/install/repositories/ookla/speedtest-cli/script.deb.sh | sudo bash
sudo apt-get install speedtest
```

## SPN removal

```text
setspn.exe -D "Entrada SPN, que precisa ser removida" "Conta de serviço ou nome do servidor"
setspn.exe -D "MSSQLSvc/KRISHNA03.SKGLAB.LOCAL:1433" "SKGLAB\SQLSvc-SQL2012"
```

