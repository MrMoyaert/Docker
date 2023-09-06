# Pi-Hosted Portainer Template V2

This repository is a collection of tutorials for hosting a variety of server applications using [Docker](https://www.docker.com/) and [Portainer](https://github.com/portainer/portainer).

### App Template for Portainer
![App Template Image](https://github.com/MrMoyaert/Docker/blob/master/apptemplate.png?raw=true)

### Apps List

See the list of apps included in this template [here](https://github.com/MrMoyaert/Docker/blob/master/docs/AppList.md).

### Installation
Run `install-docker.sh`, to install docker, and add the current user to the docker usergroup.

```
wget -qO- https://raw.githubusercontent.com/MrMoyaert/Docker/master/install_docker.sh | bash
```
You need to reboot/logout for changes to take effect

### Reboot for changes to take effect

```
sudo reboot
```

After a reboot, run `install-portainer.sh`, to install Portainer.io

```
wget -qO- https://raw.githubusercontent.com/MrMoyaert/Docker/master/install_portainer.sh | bash
# to update portainer, run this command instead
wget -qO- https://raw.githubusercontent.com/MrMoyaert/Docker/master/update_portainer.sh | bash
```

### Login to Portainer to update the App Template.

Goto pi-ip:9000 and then login

Click Settings, in the bottom-left corner, and paste the Portainer v2 json file link from below into the "App Templates" box.

You're done! Now just click App Templates and deploy applications!

#### Portainer Architecture

| Architecture | Tested OS's | URL |
| ------------ | ----------- | --- |
| Arm64   | Pi OS, Ubuntu, DietPi | https://raw.githubusercontent.com/MrMoyaert/Docker/master/template/portainer-v2-arm64.json |
