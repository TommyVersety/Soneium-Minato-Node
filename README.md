# Soneium-Minato-Node

-------------------1--------------------
sudo apt update && sudo apt upgrade -y
sudo apt install curl git jq build-essential gcc unzip wget lz4 -y
 
-------------------2--------------------
sudo apt install docker.io
 
-------------------3--------------------
docker --version
 
-------------------4--------------------
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
 
-------------------5-----------------------
git clone https://github.com/Soneium/soneium-node.git
cd soneium-node/minato
 
-------------------6-----------------------
openssl rand -hex 32 > jwt.txt
 
-------------------7-----------------------
mv sample.env .env
 
-------------------8-----------------------
nano .env
 
-------------------9-----------------------
nano docker-compose.yml
 
-------------------10-----------------------
docker-compose up -d
 
-------------------11------------------------
docker-compose logs -f op-node-minato
 
-------------------12-----------------------
docker-compose logs -f op-geth-minato
