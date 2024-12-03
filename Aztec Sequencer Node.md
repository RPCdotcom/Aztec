![Gd47gCrWQAAPHax](https://github.com/user-attachments/assets/749896b6-e519-4a5a-924a-153f74bb0ea7)

Thanks For information  : https://x.com/codeesura - Bilgilendirme için Teşekkürler : https://x.com/codeesura

##  Aztec Sequencer Node Kurulum : 

#### Gereksinimler : 
- Ubuntu 24
- 8 CPU
- 32 RAM 
- 2000 Disk - PCLE GEN 4 
- Hız : 250 Mbps 


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

#### IP adresi - Private Key - Node Portu - P2P Portunun Ayarlanması - Yeni Bir Cüzdan Oluşturun : 

```bash
export PUBLIC_IP=your_public_ip_address
export VALIDATOR_PKEY=your_validator_private_key
export NODE_PORT=8080
export P2P_PORT=40400
```

#### Validatör için Dizin : 

```bash
mkdir val1
cd val1
```

```bash
cp ../spartan/releases/rough-rhino/validator.sh .
```

#### Validator Dosyasını Çalıştıralım : 

```bash
./validator.sh
```

#### Bu komut sonrasında docker üzerinden imageleri indirip containerleri başlatacaktır. 

#### Loglara Bakmak için  : 

```bash
docker ps -a 
```

![image](https://github.com/user-attachments/assets/7d65cecc-ae3e-4527-b482-9ddde45cb35d)

###### İmleç ile gösterdiğin kısım id'niz olacaktır. Alttaki "id" kısmına "id"nizi yazın.

```bash
docker logs -f id -n 150 
```

#### Bununla birlikte son 150 log'u görebilirsiniz. 

### Discord : https://discord.gg/m4h5Ycjn

- Discordlarında Sequencer ve Prover Kanalına - adminlere cüzdan adresinizi atarak eklemelerini istemeniz gerekiyor.
