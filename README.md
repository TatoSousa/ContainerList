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

## Docker commands:
Start docker compose - **docker compose up -d**
Stop docker compose - **docker compose down**
Show logs - **docker logs [container_id]**
List containers - **docker ps**
Stop all containers - **docker stop $(docker ps -a -q)**
Remove all containers (after stop) - **docker rm $(docker ps -a -q)**
Remove all images - **docker rm -vf $(docker ps -aq) && docker rmi -f $(docker images -aq)**
