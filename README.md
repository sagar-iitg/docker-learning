# Docker
Docker Tutorial

 docker swarm init
 docker node ls


 ```
 docker commit <container_id> sagarkumar99/keycloak
 docker login
 docker push sagarkumar99/keycloak

```

```
# Download Docker Compose binary from GitHub releases using curl
curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" \
    # Save the downloaded binary to /usr/local/bin/docker-compose
    -o /usr/local/bin/docker-compose
```
```
# Make the downloaded binary executable
chmod +x /usr/local/bin/docker-compose
```
```
# Create a symbolic link from /usr/local/bin/docker-compose to /usr/bin/docker-compose
ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```
