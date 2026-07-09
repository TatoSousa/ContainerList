# Containers
This contents is exclusive for learning how to use especifics technologies, using docker tools.

Before starts change the PostgreSQL values in docker-compose.yml.

Avaiable Tools:
- Apace NiFI
- Grafana Server;
- InfluxDB - Temporal database;
- Metabase - BI Tools;
- NGinX Portable;
- PgAdmin;
- Portainer - UI for docker

## Docker commands

1. Start docker compose
``
docker compose up -d
`` 
1. Stop docker compose
``
docker compose down
``
1. Show logs
``
docker logs [container_id]
`` 
1. List containers
``
docker ps
``
1. Stop all containers 
``
docker stop $(docker ps -a -q)
``
1. Remove all containers (after stop) 
  ``
 docker rm $(docker ps -a -q)
 ``
1. Remove all images
   ``
   docker rm -vf $(docker ps -aq) && docker rmi -f $(docker images -aq)
   ``

