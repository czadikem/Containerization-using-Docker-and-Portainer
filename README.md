# Containerization using Docker and Portainer
My Containerization setup using Docker and Portainer


`sudo apt update`

`sudo apt dist-upgrade -y`

`sudo apt install qemu-guest-agent`

`sudo reboot`

`sudo apt install docker.io`

`sudo systemctl enable docker`

`sudo systemctl start docker`

`sudo systemctl status docker`

`sudo usermod -aG docker $USER`

`sudo apt install docker-compose`

## reconnect to server or logout and log back in

`sudo docker run -d \
--name="portainer" \
--restart on-failure \
-p 9000:9000 \
-p 8000:8000 \
-v /var/run/docker.sock:/var/run/docker.sock \
-v portainer_data:/data \
portainer/portainer-ce:latest`

### go to your ip-address:9000
replace ip-address with your servers ip, you can get your servers ip by doing 

`ip a`

### click disable allow collection

### click get started

### click local

### click environments

### click local

### change name to containerization

### change public ip to this servers ip address

### click stacks

### click the add stacks plus button

### name it
`containerization`




WATCHTOWER

just use the above to deploy it


REMOTELY

mkdir /home/autiboy/remotely

mkdir /home/autiboy/remotely/data

docker pull translucency/remotely


TANDOOR-RECIPES

mkdir /home/autiboy/tandoor-recipes

mkdir /home/autiboy/tandoor-recipes/postgresql

mkdir /home/autiboy/tandoor-recipes/staticfiles

mkdir /home/autiboy/tandoor-recipes/mediafiles

replace YOUR_SECRET_KEY with the  key from
base64 /dev/urandom | head -c50

replace YOUR_POSTGRES_SECRET_KEY with the  key from
base64 /dev/urandom | head -c50

docker pull vabene1111/recipes


AIRSONIC_ADVANCED

mkdir /home/autiboy/airsonic-advanced

mkdir /home/autiboy/airsonic-advanced/playlists

mkdir /home/autiboy/airsonic-advanced/podcasts

mkdir /home/autiboy/airsonic-advanced/data

mkdir /home/autiboy/airsonic-advanced/music

docker pull airsonic-advanced


JELLYFIN

mkdir /home/autiboy/jellyfin

mkdir /home/autiboy/jellyfin/library

mkdir /home/autiboy/jellyfin/tvseries

mkdir /home/autiboy/jellyfin/movies

docker pull lscr.io/linuxserver/jellyfin


NEXTCLOUD

mkdir /home/autiboy/nextcloud

mkdir /home/autiboy/nextcloud/appdata

mkdir /home/autiboy/nextcloud/data

docker pull lscr.io/linuxserver/nextcloud


SONARR

mkdir /home/autiboy/sonarr

mkdir /home/autiboy/sonarr/data

mkdir /home/autiboy/sonarr/tvseries

mkdir /home/autiboy/sonarr/downloadclient-downloads

docker pull lscr.io/linuxserver/sonarr


RADARR

mkdir /home/autiboy/radarr/

mkdir /home/autiboy/radarr/data

mkdir /home/autiboy/radarr/movies

mkdir /home/autiboy/radarr/downloadclient-downloads

docker pull lscr.io/linuxserver/radarr


LIDARR

mkdir /home/autiboy/lidarr/

mkdir /home/autiboy/lidarr/data

mkdir /home/autiboy/lidarr/music

mkdir /home/autiboy/lidarr/downloadclient-downloads

docker pull lscr.io/linuxserver/lidarr
