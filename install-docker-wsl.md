```
in cmd

wsl --version
sudo nano /etc/wsl.conf

and add
[boot]
systemd=true

```

````
sudo apt update
sudo apt install docker.io -y
sudo usermod -aG docker $USER
docker --version
exit

from cmd
wsl --shutdown

in wsl

docker run hello-world
```
