# Active Directory

## Accounts inactive more than 90 days

```powershell
Import-Module ActiveDirectory
Get-ADUser -Properties * -Filter * | ?{$_.LastLogonDate -lt (Get-Date).AddDays(-90)} | %{$_.SamAccountName}
```

## Accounts that never expire

```powershell
Get-ADUser -Filter {Enabled -eq $true -and PasswordNeverExpires -eq $true}
```

## Accounts inactive by LastLogonTimeStamp

```powershell
Get-ADUser -Filter {LastLogonTimeStamp -lt (Get-Date).AddDays(-(90)) -and enabled -eq $true} -Properties LastLogonTimeStamp
```

## Users inactive more than 12 weeks

```powershell
dsquery user -inactive 12 -limit 0 >> C:\temp\userinativo.txt
```

## Force password change in bulk

```powershell
Import-Module ActiveDirectory
Import-Csv "C:\temp\forcar.csv" | ForEach-Object {
  $samAccountName = $_."samAccountName"
  Get-ADUser -Identity $samAccountName | Set-ADUser -ChangePasswordAtLogon:$true
}
```

## Group members

```powershell
Get-ADGroupMember -Identity "NameGroup" | Export-Csv "C:\GrupoName.csv"
```

## Disable account

```powershell
Disable-ADAccount -Identity "AccountID"
```

## Disable users in bulk

```powershell
Import-Module ActiveDirectory
Import-Csv "C:\temp\desabilitar.csv" | ForEach-Object {
  $samAccountName = $_."samAccountName"
  Get-ADUser -Identity $samAccountName | Set-ADUser -Enable:$False
}
```

## Send message

```powershell
msg /server:maquina usuario * "Favor troca a sua senha urgentemente"
```

## Password expiration date

```powershell
Get-ADUser nomedousuario -Properties msDS-UserPasswordExpiryTimeComputed |
  Select-Object Name, {[datetime]::FromFileTime($_."msDS-UserPasswordExpiryTimeComputed")}
```

## Password last set

```powershell
Get-ADUser USUARIO -Properties * |
  Select-Object Name, @{Name='pwdLastSet';Expression={[DateTime]::FromFileTime($_.pwdLastSet)}}
```

## Related

- [GPO and AD](../windows/gpo-ad.md)
