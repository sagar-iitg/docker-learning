

### Create EC2 instance


```
sudo apt update
```
### Install docker on server
### Install docker-compose 
### Configure Docker Registry

```
mkdir ~/docker-registry
cd ~/docker-registry
mkdir data

# Create docker compose config file
vim docker-compose.yml

```

### Configure docker-compose.yml file

```
version: '3'

services:
  registry:
    image: registry:2  # Specifies the Docker image to use for the registry service
    ports:
      - "5000:5000"  # Exposes port 5000 on the host machine and forwards it to port 5000 in the container
    environment:
   
      REGISTRY_AUTH: htpasswd
      REGISTRY_AUTH_HTPASSWD_REALM: Registry
      REGISTRY_AUTH_HTPASSWD_PATH: /auth/registry.password


      REGISTRY_STORAGE_FILESYSTEM_ROOTDIRECTORY: /data  # Sets an environment variable to configure the storage directory
    volumes:
    ./data:/data
 - ./auth:/auth
```

      - ./data:/data  # Mounts a volume named 'data' from the host to '/data' in the container for persistent storage





http {
+ client_max_body_size 16384m;
}

sudo nginx -s reload
### Publishing images from our local machine

```

```
```

###  Nginx and SSL Setup

```

sudo apt install nginx
sudo vim etc/nginx/sites-available/<your_site>

server{

server_name your_domain.com;

    location / {
        proxy_pass                          http://localhost:5000;
        proxy_set_header  Host              $http_host;   # required for docker client's sake
        proxy_set_header  X-Real-IP         $remote_addr; # pass on real client's IP
        proxy_set_header  X-Forwarded-For   $proxy_add_x_forwarded_for;
        proxy_set_header  X-Forwarded-Proto $scheme;
        proxy_read_timeout                  900;
    }
}

# Test & Restart Nginx


# Check NGINX config
sudo nginx -t

# Restart NGINX
sudo nginx -s reload

```


### 1. SSL Certificate

```
sudo add-apt-repository ppa:certbot/certbot
sudo apt-get update
sudo apt-get install python3-certbot-nginx
sudo certbot --nginx

```

### Setting up Authentication

```
sudo apt install apache2-utils -y
mkdir ~/docker-registry/auth
cd ~/docker-registry/auth
htpasswd -Bc registry.password <username>




```



### Publishing images from our local machine

```

docker login your_domain
docker tag image <your_domain>/<repo>
docker push <your_domain>/<repo>

```