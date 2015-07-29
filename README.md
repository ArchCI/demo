# ArchCI Demo

## Introduction

Setup ArchCI service within minutes! Happy hacking!

## Tutorial

Start [MySQL](https://github.com/tobegit3hub/mysql_docker) container.

```
sudo docker run -d -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 mysql:5.7
```

Start [redis](https://github.com/tobegit3hub/redis_docker) contaienr.

```
sudo docker run -d -p 6379:6379 redis
```

Start [archci/archci](https://github.com/ArchCI/archci) server.

```
sudo docker run -d --net=host archci/archci
```

Start [archci/simple-worker](https://github.com/ArchCI/simple-worker) worker.

```
sudo docker run -d --net=host archci/simple-docker
```

## Usage

Go to <http://127.0.0.1:10010> and add new project for continuous integration.

![](./screenshot.png)
