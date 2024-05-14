# Commands

clean installation
```sh
docker rm -f windows11
sudo rm -rf ./data/*
cp custom.iso ./data/
cp ../windows/custom.iso ./data/
```

ssh passwordless
```sh
scp -P 3323 ~/.ssh/id_<>.pub docker@<ip>:'C:\ProgramData\ssh\administrators_authorized_keys'
ssh -p 3323 docker@<ip>
ssh -p 3323 docker@<ip> choco install firefox -y
```

install pwa
```sh
scp -P 3323 ~/Downloads/calc.zip docker@<ip>:'C:\Users\Docker\calc.zip'
ssh -p 3323 docker@<ip> powershell Expand-Archive 'C:\Users\Docker\calc.zip' 'C:\Users\Docker\calc'
ssh -p 3323 docker@<ip> "cd C:\Users\Docker\calc && powershell -executionpolicy bypass -File .\install.ps1"
```
