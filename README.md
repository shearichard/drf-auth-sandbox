[![Build Status](https://travis-ci.org/shearichard/drf-cc-sandbox.svg?branch=master)](https://travis-ci.org/shearichard/drf-cc-sandbox)
[![Built with](https://img.shields.io/badge/Built_with-Cookiecutter_Django_Rest-F7B633.svg)](https://github.com/agconti/cookiecutter-django-rest)

# Django Rest Framework Authentication Demonstrator

Exposing various authentication options in Django Rest Framework to allow for demonstrations and training.

# Prerequisites

- [Docker](https://docs.docker.com/docker-for-mac/install/)  

# Databases
This project is setup to use Postgres in the long term but initially uses sqlite. A flag in the [config.common](https://github.com/shearichard/drf-auth-sandbox/blob/2582af4a410917d813f1f2c1f7d5ad2206dddafe/drf-cc-sandbox/config/common.py#L8) settings module determines which is used. When the switch back to Postgres is made it will be necessary to re-run the migrations and recreat the superuser. 


# Local Development

Start the dev server for local development:
```bash
docker-compose up
```

Run a command inside the docker container:

```bash
docker-compose run --rm web [command]
```
