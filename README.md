# Ubuntu-Applications-Setup
Commands to get essential applications in Ubuntu environment
### Visual Studio Code
```sh
sudo apt update
sudo apt install software-properties-common apt-transport-https wget
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code
```
### Sublime Text
```sh
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt-get install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```
### Golang
```sh
# Install
sudo apt install golang-go 
# Uninstall
sudo apt-get remove golang-go
sudo apt-get remove --auto-remove golang-go
```
### Docker
```sh
# Install
sudo apt install docker.io
sudo systemctl status docker # show docker status
sudo systemctl start docker
sudo systemctl stop docker.socket
sudo systemctl restart docker
# docker-compose 
sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)"  -o /usr/local/bin/docker-compose
sudo mv /usr/local/bin/docker-compose /usr/bin/docker-compose
sudo chmod +x /usr/bin/docker-compose
#
sudo chown $USER /var/run/docker.sock
```
### [Videos](https://linuxhint.com/install_multimedia_codecs_ubuntu/)
