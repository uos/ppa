# UOS Mobile Robotics PPA

## Setup

```sh
curl -s --compressed "https://uos.github.io/ppa/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/uos.gpg >/dev/null
sudo curl -s --compressed -o /etc/apt/sources.list.d/uos.list "https://uos.github.io/ppa/uos.list"

sudo apt update
```
