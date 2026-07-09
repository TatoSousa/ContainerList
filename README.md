# Containers
This contents is exclusive for learning how to use especifics technologies, using docker tools.

Before starts change the PostgreSQL values in docker-compose.yml.

Avaiable Tools:
- Grafana Server;
- InfluxDB - Temporal database;
- Metabase - BI Tools;
- NGinX Portable;
- Apace NiFI
- PgAdmin;
- Portainer - UI for docker

## Docker commands

1. Start docker compose
``sh
docker compose up -d
`` 
1. Stop docker compose
``sh
docker compose down
``
1. Show logs
``sh
docker logs [container_id]
`` 
1. List containers
``sh
docker ps
``
1. Stop all containers 
``sh
docker stop $(docker ps -a -q)
``
1. Remove all containers (after stop) 
  ``sh
 docker rm $(docker ps -a -q)
 ``
1. Remove all images
   ``sh
   docker rm -vf $(docker ps -aq) && docker rmi -f $(docker images -aq)
   ``

