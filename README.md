# Active Directory Home Lab SetUp

## 00 - Instal VM's

1. Installed Windows server 2022
2. Installed Windows 11

## 01 - Install DC

1. Use `Sfconfig` to:
    - Change hostname
    - Change the IP Address to static
    - Change the DNS server to own Server IP address.

2. Install AD Window Feature

```shell
Get-WindowsFeature | ? {$_.Name -like "AD*"}

Install-WindowsFeature AD-Domain-Services -IncludeManagementTools  
```

