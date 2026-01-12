# UOS Mobile Robotics PPA

## Setup

```sh
curl -fsSL "https://uos.github.io/ppa/KEY.gpg" | gpg --dearmor \
  | sudo tee /usr/share/keyrings/uos-archive-keyring.gpg >/dev/null
echo "deb [signed-by=/usr/share/keyrings/uos-archive-keyring.gpg] https://uos.github.io/ppa ./" \
  | sudo tee /etc/apt/sources.list.d/uos.list
sudo apt update
```

