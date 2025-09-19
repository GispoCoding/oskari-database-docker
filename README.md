# oskari-database-docker

This docker container provides a minimal working database setup for Oskari, intended for use in Oskari development. It initializes the Oskari database following the guidelines outlined in the [Oskari documentation](https://oskari.org/documentation/docs/latest/2-Setup-instructions#Setup-database).

## Requirements

- Docker Compose or podman-compose (tested with Podman 4.9.3 and podman-compose 1.0.6)

## Steps to run

1. Copy the environment template

- copy .env.template to .env

2. Edit environment variables

- edit environment variables in .env
  - OSKARI_DB_PORT - database port
  - OSKARI_DB_USER - username for the Oskari database
  - OSKARI_DB_PASSWORD - password for the Oskari database user

3. Start the database

- ```docker compose up db``` or ```podman-compose up```
