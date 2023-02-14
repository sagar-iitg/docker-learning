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

