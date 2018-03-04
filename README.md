# README

You can refer to the following instruction to build a simple XMPP ejabberd service. 

# Prerequisites

- Docker Engine
- Docker Compose toolkit, ref: https://docs.docker.com/compose/install/



# Installation

Download the git source

```sh
$ git clone git@github.com:erichsu/slymbridge-xmpp.git
```



Start the docker container

```sh
$ cd slymbridge-xmpp
$ docker-compose up -d

# check process
$ docker-compose ps

# stop 
$ docker-compose down

# restart
$ docker-compose restart
```



Enter docker container

```sh
# lanuch bash shell in container and attach
$ docker-compose exec ejabberd bash

# in container, you can execute the CLI
$ bin/ejabberdctl modules_update_specs
$ bin/ejabberdctl register admin localhost password
```



