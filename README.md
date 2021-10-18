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

## add to path
ls -a ~/
nano ~/.zshrc # if do not have it 
echo "alias subl='open -a /Applications/Sublime\ Text.app'" >> ~/.zshrc
```
### Intellij
* [install intellij ubuntu linux](https://itsfoss.com/install-intellij-ubuntu-linux/)
```sh
sudo snap install intellij-idea-community --classic
```
### Conda
[Install Conda on linux](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html)
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
### Golang
```sh
# Install
sudo apt install golang-go 
# Uninstall
sudo apt-get remove golang-go
sudo apt-get remove --auto-remove golang-go
```
### Java
* [amazon correto](https://aws.amazon.com/corretto/)
### C#
[how-to-install-dotnet-cli-tools-on-ubuntu-18-10-for-vscode](https://stackoverflow.com/questions/52988294/how-to-install-dotnet-cli-tools-on-ubuntu-18-10-for-vscode)
```sh
# paste line below in `/etc/apt/sources.list`
deb [arch=amd64] https://packages.microsoft.com/ubuntu/18.04/prod bionic main
sudo apt-get update
sudo apt-get install dotnet-sdk-5.0
```
### [Videos](https://linuxhint.com/install_multimedia_codecs_ubuntu/)
