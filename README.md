# UOS Mobile Robotics PPA

> [!NOTE]  
> The PPA moved to codeberg to fix some problems with CI.
> To use the new PPA, overwrite the list file with:
> ```sh
>  echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/uos-archive-keyring.gpg] https://uos-robotics.codeberg.page/ppa/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" \
>  | sudo tee /etc/apt/sources.list.d/uos.list
> ```

Precompiled packages.

## Setup

### Ubuntu

- 22.04 LTS (jammy)
- 24.04 LTS (noble)

```sh
curl -fsSL "https://uos-robotics.codeberg.page/ppa/ubuntu/key.gpg" | gpg --dearmor \
  | sudo tee /usr/share/keyrings/uos-archive-keyring.gpg >/dev/null
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/uos-archive-keyring.gpg] https://uos-robotics.codeberg.page/ppa/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" \
  | sudo tee /etc/apt/sources.list.d/uos.list
sudo apt update
```
