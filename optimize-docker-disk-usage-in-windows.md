
Stop docker and wsl
```
> net stop com.docker.service
> taskkill /IM "docker.exe" /F
> taskkill /IM "Docker Desktop.exe" /F
> wsl --shutdown
```

Optimize-VHD
```
> Optimize-VHD -Path $Env:LOCALAPPDATA\Docker\wsl\data\ext4.vhdx -Mode Full
```
