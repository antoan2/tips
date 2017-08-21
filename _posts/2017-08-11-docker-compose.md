---
layout: post
title: docker compose configuration override
author: Alexandre B.
tags: [docker,docker-compose]
---
## Override your docker-compose.yml

The trouble in the `docker-compose.yml` and `docker-compose-prod.yml` is that you have to repeat common configurations.

To avoid that, you can use the override feature of docker-compose :

A `docker-compose.override.yml` file will override the configuration.

We can use `docker-compose.override.yml` for the DEV env, and a `docker-compose.prod.yml for production :

`docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d`


_source: https://docs.docker.com/compose/extends/#example-use-case_
