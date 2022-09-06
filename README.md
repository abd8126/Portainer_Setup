# Portainer_Setup_On_Linux
- Install Docker in OS
## Create Docker Volume for portainer
- docker volume create portainer_data
## Run Dcoker with volume of portainer_data and expose the port. 
- docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:2.11.1

