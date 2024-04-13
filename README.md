# docker-portainer
docker &amp; portainer


How to Install Docker and Portainer on Debian

1. Install and start docker by running the commands below.

sudo apt install docker.io
sudo systemctl start docker

2. Download and run Portainer 2.0 by running the commands below.

sudo docker run -d -p 8000:8000 -p 9000:9000 -p 9443:9443 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest

3. This will install Docker and it will be accessible by the workstation’s IP address and port 9000. When you get there, create a username and password.

http://[WORKSTATION_IP_ADDRESS]:9000

4. Select Docker and Connect.


5. Select Local.
