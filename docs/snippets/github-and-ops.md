# GitHub and ops notes

## Git basics

- `git clone` copies files
- `git add` stages changes
- `git commit` creates a new snapshot

Source:
- https://git-scm.com/book/en/v2

## SoapUI

1. Insert project name and address.
![SoapUI project and address](https://user-images.githubusercontent.com/48725940/235219218-56814adb-e644-4771-91f1-cf7538adf95f.png)
2. In request, select auth.
![SoapUI auth selection](https://user-images.githubusercontent.com/48725940/235219621-62b0416c-0306-40de-a248-3aa15fd0847d.png)
3. Use dynamic domain registration when needed.
- https://spdyn.de/

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

- https://sudeeptaganguly.wordpress.com/2015/08/03/removing-a-spn-ent
