# alpine-ss
---
## [![](https://badge.imagelayers.io/snakeliwei/alpine-ss:latest.svg)](https://imagelayers.io/?images=snakeliwei/alpine-ss:latest 'Get your own badge on imagelayers.io')
### docker-shadowsocks
>This Dockerfile builds an image with the Python implementation of shadowsocks. Based on alpine image.

Quick Start:
This image uses ENTRYPOINT to run the containers as an executable.
```bash
$ docker run -d -p 1984:1984 snakeliwei/alpine-ss -s 0.0.0.0 -p 1984 -k $SSPASSWORD -m aes-256-cfb
```
You can configure the service to run on a port of your choice. Just make sure the port number given to Docker is the same as the one given to shadowsocks. Also, it is highly recommended that you store the shadowsocks password in an environment variable as shown above. This way the password will not show in plain text when you run docker ps.

For more command line options, refer to the shadowsocks documentation
