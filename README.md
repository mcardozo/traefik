# Traefik

<p align="center">
<img src="docs/img/traefik-architecture.png" alt="Traefik" title="Traefik" />
</p>

This git repository contains basic structure for create
proxy rules with Traefik of your docker services

## Stack technologies

- [Docker](https://docs.docker.com/engine/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Traefik](https://doc.traefik.io/traefik/)

## Get started

1. Set values corresponding for email, host and add your
services. Default is **flask**

		$ vi compose/production/traefik/traefik.yml

2. Build Trafik image

		$ export COMPOSE_FILE=production.yml

		$ docker-compose build

3. Run Traefik

		$ docker-compose up -d

## Local

You can testing Traefik in your local environment

1. Set values corresponding in _traefik.yml_

		$ vi compose/local/traefik/traefik.yml

2. Build Trafik image

		$ export COMPOSE_FILE=local.yml

		$ docker-compose build

3. Run Traefik

		$ docker-compose up
