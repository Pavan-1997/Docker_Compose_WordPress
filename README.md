# Docker Compose to deploy a WordPress application

1. Create a EC2 Ubuntu instance and open the below ports 


2. Install docker by using the below commands
```
sudo apt update -y

sudo apt install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"

apt-cache policy docker-ce

sudo apt install docker-ce

sudo usermod -aG docker $USER

sudo systemctl status docker 
```

3. Install docker compose by using the below commands 
```
sudo apt install docker-compose
```

4. Use the below docker compose file to run
```
sudo docker-compose --version
```

5. Run the Docker Compose file
```
sudo docker-compose up -d
```

6. Now check the port of the app using below
```
sudo docker-compose ps
```

7. Access the app on Public IP using port 80 
