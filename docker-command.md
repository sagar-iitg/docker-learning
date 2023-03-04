```

docker run -d --name mysqldb -p 3308:3306 -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=db_name  mysql
docker run -it --name store -p 9091:9090 -e MYSQL_HOST=mysqldb -e MYSQL_PORT=3306 ecom-app
```
