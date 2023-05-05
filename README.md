# create-k3s-uninstall
Script which creates k3s-unininstall.sh from source code in repository `https://github.com/k3s-io/k3s/blob/master/install.sh`

This script comming handy especially when you are using k3s server from source, esecially when tou run it whithout systemd (on WSL for example).

Normal installation will also create `k3s-uninstall.sh` script on `/usr/local/bin`.

But when you use k3s server from binary you may not have such script in required path, thus using this script you can have `k3s-uninstall.sh` directly from source code.

Script will parse k3s intallation script and creates `k3-uninstall.sh` script.

## Usage
Clone repository, go into repository folder and the run following:

```
./create-k3s-uninstall.sh
sudo mv ./k3s-uninstall.sh /usr/local/bin/k3s-uninstall.sh
```
