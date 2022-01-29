# Ubuntu Setup Notes

```sh
sudo apt-get install git -y

sudo snap install docker

sudo addgroup --system docker 
sudo adduser $USER docker 
newgrp docker 
sudo snap disable docker 
sudo snap enable docker

sudo snap install code --classic

sudo snap install gitkraken --classic

sudo snap install insomnia

sudo snap install termius-app

#Node Version Manager
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

sudo add-apt-repository ppa:bamboo-engine/ibus-bamboo 
sudo apt-get update 
sudo apt-get install ibus ibus-bamboo --install-recommends 
ibus restart 
# Setup ibus-bamboo is default typing engine.
env DCONF_PROFILE=ibus dconf write /desktop/ibus/general/preload-engines "['BambooUs', 'Bamboo']" && gsettings set org.gnome.desktop.input-sources sources "[('xkb', 'us'), ('ibus', 'Bamboo')]"

sudo snap install spotify

sudo snap install foobar2000

```
