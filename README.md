# Base Application

OBS.: If in your conf docker compose command is used as "docker-compose", please, make adjustments in code before continue.
This project default is "docker compose".

## Steps 

### Clone repository

### Enter folder

`cd docker-env/nginx`

### Copy and edit your .confs

`cp .site.conf.example .site.conf`

### Add the app URL to your hosts

`vi /etc/hosts/`

`127.0.0.1 project_folder.desenv`

### Run docker compose

`docker compose -f ../docker-compose.yaml up -d`

### Install your APPs properly

`docker exec -it docker-env-php81-fpm bash`

### Testing

`http://project_folder.desenv:8080/`

Must show your project home page, repeat the .conf step and beyond to add more APPs
