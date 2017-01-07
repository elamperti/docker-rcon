# Minecraft rcon [![Docker Automated build](https://img.shields.io/docker/automated/elamperti/docker-rcon.svg)](https://hub.docker.com/r/elamperti/docker-rcon/)

This is an Alpine based rcon container, using [mcrcon](https://github.com/Tiiffi/mcrcon) as client.

## Usage
Run it specifying host, port and password along with a command (or `-t` for a interactive terminal):

```
docker run elamperti/docker-rcon -H <server_ip> -P <port> -p <password> "say Hello world" save-all
```

The client is able to take the server address, port and password from environment variables `MCRCON_HOST`, `MCRCON_PORT` and `MCRCON_PASS`.
