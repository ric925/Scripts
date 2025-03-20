#Install Docker

sudo apt-get update
sudo apt install curl

curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh ./get-docker.sh


curl -fsSL https://desktop.docker.com/linux/main/amd64/docker-desktop-amd64.deb -o docker-desktop-amd64.deb
sudo apt-get update
sudo apt-get install ./docker-desktop-amd64.deb

#Install Portainer
docker volume create portainer_data
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:lts
