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



```

sudo apt update
sudo apt install docker.io -y
docker --version

vi .bashrc

# Start Docker daemon automatically when logging in if not running.
RUNNING=`ps aux | grep dockerd | grep -v grep`
if [ -z "$RUNNING" ]; then
    sudo dockerd > /dev/null 2>&1 &
    disown
fi

sudo usermod -aG docker $USER

```
