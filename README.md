## Install Docker Engine on Ubuntu

    1) sudo apt-get update
    2) sudo apt-get install \
        apt-transport-https \
        ca-certificates \
        curl \
        gnupg-agent \
        software-properties-common

    3)  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add
    4)  sudo apt-key fingerprint 0EBFCD88
    5)  sudo add-apt-repository \
        "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
        $(lsb_release -cs) \
        stable"
    6)  sudo apt-get update
    7)  sudo apt-get install docker-ce docker-ce-cli containerd.io
    8)  apt-cache madison docker-ce

## 2. Install Docker-Compose

    0)  sudo apt-get update
    1)  sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    2)  sudo chmod +x /usr/local/bin/docker-compose
    3)  sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
    4)  sudo docker-compose --version

## 3. Install Git

    0)  sudo apt-get update
    1)  sudo apt-get install git

## 4. Clone Project & docker-compose.yml file

    1) sudo git clone https://github.com/nathakrit061103jnt/docker-compose-mqtt-broker.git docker-compose-mqtt-broker
    2) cd docker-compose-mqtt-broker
    3) sudo docker-compose up -d

## Node-Red Port 1880

## Mqtt Broker eclipse-mosquitto Port 1883

## portainer Port 9000
