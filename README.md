# Guideline to install Docker on an Ubuntu machine on Azure

Here is the guideline that I combined when I was trying to install [Docker](https://www.docker.com/) on an [Ubuntu](https://ubuntu.com/) machine on [Azure](https://portal.azure.com)

_PS : I need to run [Docker](https://www.docker.com/) on a VM on [Azure](https://portal.azure.com) to run [Remote DevContainers](https://github.com/polatengin/project-standards/blob/master/DevContainers.md) on it. So, I wouldn't need to install and run [Docker](https://www.docker.com/) on my machine anymore. If you follow below guideline and install [Docker](https://www.docker.com/) on a machine on [Azure](https://portal.azure.com), you can run [Visual Studio Code](https://code.visualstudio.com) on you machine and actual DevContainer on [Azure](https://portal.azure.com). Also, you can benefit beast hardware specs you can find on [Azure](https://portal.azure.com), such as, enourmous amount of CPU cores, gigabytes of RAM, fast GPUs, etc._

```bash
apt-get install -y apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

apt-get update

apt install docker.io

systemctl start docker

systemctl enable docker
```
