# Docker composed [Sensu + Uchiwa]

## Prerequisites

You need to install :

- [docker-machine](https://docs.docker.com/machine/install-machine/)
- [docker-compose](https://docs.docker.com/compose/install/)

## Content

5 docker containers + 1 docker compose file :

- Sensu : ... and dependencies (rabbitmq, redis)
- Uchiwa : sensu dashboard
- Test-container : send container memory datas to Sensu

## Install & Run

We assume that you got at least one docker machine called _docker-vm_. If not, you can change it in the cmdline.

> sh start-sensu.sh docker-vm

## Check Uchiwa dashboard

> open http://$(docker-machine ip docker-vm)/