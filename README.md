# bancho.py
Running on Ubuntu 22.04

MySQL : 5.7

## Don't ask. just ctrl + c , ctrl + v
```
sudo apt-get update
git clone https://github.com/osuAkatsuki/bancho.py
cd bancho.py
sudo apt install -y docker
sudo apt-get update
sudo apt-get install build-essential
cp .env.example .env
cp logging.yaml.example logging.yaml
nano .env
sudo apt install nginx
sudo ./scripts/install-nginx-config.sh
make build
make run
make run-bg


Docker compose
sudo apt install -y docker.io
sudo apt install docker-compose-v2

mkdir -p ~/.docker/cli-plugins/
curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
chmod +x ~/.docker/cli-plugins/docker-compose
docker compose version

fuck docker-compose

no sudo docker
sudo usermod -aG docker $USER
sudo reboot

```
## License

**bancho.py** is licensed under the [MIT License](https://opensource.org/license/mit/). Please see the [LICENSE](https://github.com/osuAkatsuki/bancho.py/blob/master/LICENSE) file for more information.
