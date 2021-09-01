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
```
