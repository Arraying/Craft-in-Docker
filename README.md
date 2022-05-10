# Craft-In-Docker

This allows an installation of Craft CMS on the host machine while serving through Docker.

## Database

A PostgreSQL database `craft` with username and password `postgres` is provided. It can be connected to at `database:5432`.

## Installation

Clone the repository and switch to the folder:
```
$ git clone git@github.com:Arraying/Craft-in-Docker.git CID && cd CID
```
[Install Craft CMS](git@github.com:Arraying/Craft-in-Docker.git) and use `projectroot` as `my/project/path`.
Follow the installation instructions.

Spin up the server:
```
$ docker-compose up -d
```

Craft will be served on `localhost:8000`. Finalize the installation in the browser.