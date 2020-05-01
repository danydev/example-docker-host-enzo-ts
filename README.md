# ENZO-TS docker host

Run an **unofficial** docker container for [ENZO-TS](https://www.enzobot.com). Use at your own risk.  

## Setup
- Run ENZO-TSC with UI to configure your account, and setup the client.
- Put the resulting configuration file (named `enzo_tsc_config.json`) in this repository path `mounted-files\config\enzo_tsc_config.json`. The file can be located by clicking `File\Open Profile Folder` in ENZO-TSC UI.
- Run `docker-compose up -d`

## Logs
Logs can be inspected on a running container with `docker logs -f enzo-ts`. All logs are stored in `mounted-files\logs` that is a mounted volume in the container, thus logs are preserved when destroying the container.

## How to do my own build?
You can do your own building using [docker-build-enzo-ts](https://github.com/danydev/docker-build-enzo-ts)
