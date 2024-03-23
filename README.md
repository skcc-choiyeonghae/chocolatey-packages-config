My Chocolatey Packages.config
----
This repo was created for the purpose of backup my personal settings.
## Chocolatey Installation:

1. Run PowerShell as an **administrator**.
2. Enter the following command.
```ps1
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
3. Once the installation is complete, type `choco -v` to verify the installation. ✔

## Packages Installation:
```ps1
# Clone packages.config file
Invoke-WebRequest -Uri https://raw.githubusercontent.com/supex0hae/chocolatey-packages-config/main/packages.config -OutFile packages.config

# Install packages
choco install .\packages.config -y
```
