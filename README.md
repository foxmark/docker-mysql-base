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

## Override/change configuration (Optional)

Rename and inspect ```docker-compose.override.yml``` file

> Note: You can use this file to make local configuration changes.

```sh
cp docker-compose.override.example.yml docker-compose.override.yml
```

```sh
nano docker-compose.override.yml
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
f3faaa6f53e7   mysql:8.0.35              "docker-entrypoint.s…"   15 minutes ago   Up 15 minutes               33060/tcp, 0.0.0.0:3306->3306/tcp, :::3306->3306/tcp   mysql_mysql8_container
```
