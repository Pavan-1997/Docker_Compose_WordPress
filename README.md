# Docker Compose to deploy a WordPress application

1. Create an EC2 Ubuntu instance and open the port 80 and 3306 


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
![image](https://github.com/Pavan-1997/Docker_Compose_WordPress/assets/32020205/0570c5b6-f6a6-4957-8191-14c500a0a55e)


7. Access the app on Public IP using port 80 

![image](https://github.com/Pavan-1997/Docker_Compose_WordPress/assets/32020205/05a4acc0-0b44-49ed-9040-7327e36d75ee)
