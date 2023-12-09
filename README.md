# Welcome to Solsgate

This is a repo for new users getting started with Docker.

You can try it out using the following command.
```
docker run -d -p 8080:80 --name webserver solsgate
```
And open `http://localhost:8080` in your browser.

# Building

Maintainers should see [MAINTAINERS.md](MAINTAINERS.md).

Build and run:
```
docker build -t solsgate . 
docker run -d -p 8080:3000 --name webserver solsgate
```
Open `http://localhost:8080` in your browser.
