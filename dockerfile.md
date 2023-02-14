## Example


```
FROM python:3.9
WORKDIR app
COPY . /app
RUN pip install -r requirements.txt
EXPOSE 8001
CMD ["python","manage.py","runserver","0.0.0.0:8001"]
```

## Example

```
FROM openjdk:13-jdk-alpine3.10
COPY . /app/bin
ADD /folder /app/folder
ENV PATH "$PATH:/app/bin/sk.jar"
ENV CLASSPATH "$CLASSPATH:/app/bin/sk.jar"
CMD sh
```

## Example

```
FROM tomcat:9.0-alpine
MAINTAINER SAGAR KUMAR
EXPOSE 8080
ADD project.war /usr/local/tomcat/webapps
CMD["catlina.sh","run"]

```

## Example
```
FROM tomcat:9.0.71-jre11-temurin-focal
MAINTAINER SAGAR KUMAR
EXPOSE 8080

ADD FoodApp.war /usr/local/tomcat/webapps

CMD ["catalina.sh","run"]

```
## Example


```
FROM nginx:alpine
LABEL maintainer="Sagar Kumar"
COPY index.html /usr/share/nginx/html
WORKDIR /apps


```


## Example

```
FROM alpine
LABEL maintainer="SK"
RUN apt update && apt install nginx -y
WORKDIR /apps
COPY ./index.html .
CMD ["service","nginx","start"]

```







