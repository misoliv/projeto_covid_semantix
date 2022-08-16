Projeto final do curso de Engenharia de Dados – Semantix.

Os dados utilizados neste projeto foram coletado no site: https://covid.saude.gov.br/


INSTALAÇÃO DOCKER E DOCKER-COMPOSE 

#Docker:
sudo apt update
sudo apt upgrade
sudo apt-get install  curl apt-transport-https ca-certificates software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update
sudo apt install docker-ce
sudo systemctl status docker
Check:
sudo docker run hello-world
Sem sudo:
sudo usermod -aG docker $(whoami)
sudo reboot

#Docker-compose:
sudo curl -L https://github.com/docker/compose/releases/download/1.25.3/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
Check:
docker-compose --version
mkdir helloTeste

- Cluster:
 
git clone http://github.com/rodrigo-reboucas/docker-bigdata.git.spark

- Imagens:
 
docker-compose-fdocker-compose-completo.yml pull

- Iniciar Cluster Big Data:
 
docker-compose -f docker-compose-parcial.yml up -d
