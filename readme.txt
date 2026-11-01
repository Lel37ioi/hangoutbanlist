sudo apt update
sudo apt install docker.io docker-compose-v2
sudo systemctl enable --now docker
sudo usermod -aG docker $USER
mkdir ~/nakama && cd ~/nakama
wget https://raw.githubusercontent.com/heroiclabs/nakama/master/docker-compose.yml
docker compose up
