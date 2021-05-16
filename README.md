# ENZO-TS docker host

Run an **unofficial** docker container for [ENZO-TS](https://www.enzobot.com). Use at your own risk.  

## Setup
- To produce the config files, the simplest way is to run ENZO-TSL with UI, so you can setup the client. Then you put the resulting configuration directories (named `enzo-tsl` and `enzo-tsc`) in this path `mounted-files\config`. The folder can be located by clicking `File\Open Profile Folder` in ENZO-TSC and ENZO-TSL UI.
- Update `docker-compose.yml` to use the latest image tag available. You can see the tags available [here](https://hub.docker.com/r/dorru/enzo-ts/tags?page=1&ordering=last_updated)
- Run `docker-compose up -d`

## Logs
Logs can be inspected on a running container with `docker logs -f enzo-ts`. All logs are stored in `logs` subfolders inside `config\enzo_tsl` and `config\enzo_tsc`.

## I do not trust your build, how to do my own build?
You can do your own building using [docker-build-enzo-ts](https://github.com/danydev/docker-build-enzo-ts)
