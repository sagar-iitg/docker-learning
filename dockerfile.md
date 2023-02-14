# Example 1

```
FROM python:3.9
WORKDIR app
COPY . /app
RUN pip install -r requirements.txt
EXPOSE 8001
CMD ["python","manage.py","runserver","0.0.0.0:8001"]
```

# Example 2

```
FROM openjdk:13-jdk-alpine3.10
COPY . /app/bin
ADD /folder /app/folder
ENV PATH "$PATH:/app/bin/sk.jar"
ENV CLASSPATH "$CLASSPATH:/app/bin/sk.jar"
CMD sh
```

# Example 3

```
FROM tomcat:9.0-alpine
MAINTAINER SAGAR KUMAR
EXPOSE 8080
ADD project.war /usr/local/tomcat/webapps
CMD["catlina.sh","run"]

```
