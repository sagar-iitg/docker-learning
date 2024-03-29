## Example1
```
version: '3.9'

services:
  web:
    build: .
    ports:
      - "8001:8001"
      
      
      
```


## Example2
```
version: '3.9'

services:
  web:
    image: "sagarkumar99/node-todo-jenkins:latest"
    ports:
      - "8000:8000"


```
## Example3

```
version: '3.7'

services:
  django-app:
    image: sagarkumar99/react-django-todo-app:tagname
    ports:
      - "8001:8001"
  mysql-db:
    image: mysql:latest
    ports:
      - "3306:3306"
      
      
```

## Example 4

```
version: '3.3'

services:
  db:
    image: 'monngo:4.0'
    command: monogod --quiet --logpath=/dev/null
    ports:
      - "27017:27017"
    volumes: 
      - mongodb: /data/db
    
  backend:
    container_name: api
    ports:
      - "4000:4000"
    build:
      context: ./
      dockerfile: ./services/api/app/Dockerfile
    links:
      - db
  
  frontend:
    container_name: ui
    ports:
      - "3000:3000"
    build:
      context: ./
      dockerfile: ./services/ui/app/Dockerfile


volumes:
  mongodb:
    driver: local




``