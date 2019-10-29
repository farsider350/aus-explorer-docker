# aus-explorer-docker
 Easy to install docker image to run the AUS explorer

 Install dependences (docker & docker compose) (may vary for 18.04 machines)

Docker:
sudo apt-get update && sudo apt-get install -y apt-transport-https ca-certificates curl software-properties-common vim && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" && sudo apt-get update && sudo apt-get install -y docker-ce

Docker-compose:

sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

docker-compose --version


git clone https://github.com/farsider350/aus-explorer-docker 

cd aus-explorer-docker
cd explorer
sudo docker-compose up --build -d
off the top of my head I believe thats everything if you're just building the explorer as I have already created and uploaded a aus image to docker.
https://cloud.docker.com/u/twinkykms/repository/docker/twinkykms/australia-cash

cd aus-docker 
sudo docker build -t dockeruser/docker-repo:release_name .