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
