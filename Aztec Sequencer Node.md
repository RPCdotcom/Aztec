![Gd47gCrWQAAPHax](https://github.com/user-attachments/assets/749896b6-e519-4a5a-924a-153f74bb0ea7)


##  Aztec Sequencer Node Kurulum : 

#### Gereksinimler : 
- Ubuntu 24
- 4 CPU
- 8 RAM 
- 200 Disk


#### Güncelleme : 

```bash
sudo apt update -y && sudo apt upgrade -y
```

```bash
sudo apt install ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen unzip lz4 -y
```

#### Docker : 

```bash
sudo apt install docker.io
```

```bash
sudo systemctl start docker
sudo systemctl enable docker
```

```bash
sudo groupadd docker
sudo usermod -aG docker $USER
```

```bash
newgrp docker
```

#### Aztec Reposunu Klonlayalım : 

```bash
git clone https://github.com/AztecProtocol/aztec-packages && cd aztec-packages
```

#### Validatör için Dizin : 

```bash
mkdir val1
cd val1
```

```bash
cp ../spartan/releases/rough-rhino/validator.sh .
```
