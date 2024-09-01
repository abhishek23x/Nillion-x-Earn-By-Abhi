# Nillion-x-Earn-By-Abhi

**Use Command One By One:**
```
sudo apt update -y

```
```
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y

```

```

sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

```

```
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

```
```

sudo apt update -y

```

```
apt-cache policy docker-ce

```
```
sudo apt install docker-ce -y

```
```
sudo usermod -aG docker ${USER}
su - ${USER}
groups
```

```

docker --version

```
```
docker pull nillion/retailtoken-accuser:v1.0.0

```

```
mkdir -p nillion/accuser

```
```

docker run -v .\nillion\accuser:/var/tmp nillion/retailtoken-accuser:v1.0.0 initialise

```

**Final Command To Run**
```
docker run -v ./nillion/accuser:/var/tmp nillion/retailtoken-accuser:latest accuse --rpc-endpoint "https://testnet-nillion-rpc.lavenderfive.com" --block-start 5107613

```

**Backup Private Key**
```
cat ~/nillion/accuser/credentials.json
```

👉🏻**Join Our Telegram:** https://t.me/EarnByAbhi23

👉🏻**Follow Our Twitter:** https://x.com/EarnByAbhi
