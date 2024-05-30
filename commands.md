# Commands

### Set SSH Passwordless
```sh
scp -P 3322 ~/.ssh/id_<>.pub docker@<ip>:'C:\ProgramData\ssh\administrators_authorized_keys'
```

### Connect via SSH
```sh
ssh -p 3322 docker@<ip>
```

### Install App through SSH and Chocolatey
```sh
ssh -p 3322 docker@<ip> choco install firefox -y
```

### Copy local file through SSH
```sh
scp -P 3322 ~/Downloads/calc.zip docker@<ip>:'C:\Users\Docker\calc.zip'
```

### Extract files through SSH with PowerShell
```sh
ssh -p 3322 docker@<ip> powershell Expand-Archive 'C:\Users\Docker\calc.zip' 'C:\Users\Docker\calc'
```

### Install PWA through SSH with PowerShell
```sh
ssh -p 3323 docker@<ip> "cd C:\Users\Docker\calc && powershell -executionpolicy bypass -File .\install.ps1"
```

### Perform a clean reinstallation
```sh
docker rm -f windows11
sudo rm -rf ./data/*
# In case of having a custom Win11.iso
cp ../windows/custom.iso ./data/
```
