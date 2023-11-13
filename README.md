# Installation

## Clone project

```sh 
git clone https://github.com/foxmark/docker-mysql-base.git
```

## Change directory

```sh
cd docker-mysql-base
```

## Edit Configuration

#### Copy and Inspect ```.env``` file and make config changes

```sh
cp .env.example .env
```

```sh
nano .env
```

## Start docker services

```sh
docker-compose up
```

> Note: use ```-d``` to fee the terminal

## Validate installation

Run:

```sh
docker ps --all
```
Output should look a bit like this:

```
CONTAINER ID   IMAGE                     COMMAND                  CREATED          STATUS                      PORTS                                                  NAMES
f3faaa6f53e7   mysql:8.0.35              "docker-entrypoint.s…"   15 minutes ago   Up 15 minutes               33060/tcp, 0.0.0.0:3312->3306/tcp, :::3312->3306/tcp   mysql_mysql8_container
```
