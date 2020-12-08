# docker-wallabag

Docker-compose setup to run [Wallabag](https://wallabag.org) within Jason Wilder's [nginx proxy setup](https://github.com/nginx-proxy/nginx-proxy).

This setup can be used with the Docker image provided by Wallabag itself (https://github.com/wallabag/docker/).

However, as that image is based on an old Alpine Linux version, an additional Dockerfile using the latest Alpine version is provided here.
A corresponding PR is opened (https://github.com/wallabag/docker/pull/221). That image also contains changes to force a DB migration
on every container start.

## Configuration

Check the `docker-compose.override.yml` in the `samples` directory. Copy this file in the main directory, set the variables according to your local preferences and start up the docker-compose configuration using `docker-compose up -d`.
