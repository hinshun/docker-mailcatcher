# docker-mailcatcher
Mailcatcher container on official ruby image. [DockerHub](https://hub.docker.com/r/hinshun/mailcatcher/)

Run using `docker run --rm hinshun/mailcatcher` and visit http://docker-machine-ip:1080.
Or add in compose file to link with a rails web server for example:
```yml
web:
  image: your-web-app
  links:
    mailcatcher

mailcatcher:
  image: hinshun/mailcatcher
  ports:
    - 1080:1080
```
