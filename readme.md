## Powershell

```powershell
Set-ExecutionPolicy RemoteSigned #as admin

#Install Bitwarden
winget install --id 9PJSDV0VPK04 --source msstore  --force --accept-source-agreements --accept-package-agreements
#Install Chrome
winget install --id Google.Chrome --source msstore  --force --accept-source-agreements --accept-package-agreements
#Install FireFox
winget install --id Mozilla.Firefox_n80bbvh6b1yt2 --source msstore  --force --accept-source-agreements --accept-package-agreements
#Install windows Terminal
winget install --id Microsoft.WindowsTerminal --source msstore  --force --accept-source-agreements --accept-package-agreements
```

 ## Windows Subsystem for Linux
 ```powershell
#Install WSL
winget install wsl -h --force --accept-source-agreements --accept-package-agreements

#Install Kali to WSL
wsl --install -d kali-linux --yes

# Starts Kali
kali
```

## Setup Kali
 ```linux
#Install everything for GUI, 
touch ~/.hushlogin && sudo apt-get update && sudo apt-get full-upgrade -y && sudo apt install -y kali-win-kex && echo "alias gui='kex --win -s'" >> ~/.bashrc && source ~/.bashrc
#then just tupe "gui" and give it a password. 
```
