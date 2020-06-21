# WordPress Starter with Docker

This project help you to easily configure and run new WordPress environment. 
This container includes Wordpress with Apache server, MySql and PhpMyAdmin.

# Files

## Content

- *docker-compose.yml* : Docker configuration
- *phpconfiguration/* : Php configuration to avoid upload errors. Edit to upgrade *upload_max_filesize* and *memory_limit*
- *wordpress/* : Extract your wordpress files here
- *data/* : Databases files

# Prerequisite

Before starting, you must first install on your device :

- Docker : [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/).
- docker-compose : included by default with Docker for Windows. Check your installation with 
`docker-compose -v`

And download the last WordPress version :

- Wordpress : [https://fr.wordpress.org/download/](https://fr.wordpress.org/download/)


# QuickStart

## Configuration

1. Get this repo : download it or get it with 
`git clone https://github.com/VictorFavreau/wordpress-starter-docker.git` 

2. Extract the content the downloaded WordPress archive in the wordpress folder.
3. Start the docker-compose container by executing this command in the main directory (with the *docker-compose.yml* file)
`docker-compose up` (with logs)
or
`docker-compose up -d` (detached mode without logs)

Use `docker-compose down`  to stop the container


## PhpMyAdmin

You can now access to you database with PhpMyAdmin on [localhost:8080](http://localhost:8080)

> **Note:** By default your db username was **wordpress** and you password was **wordpress**.

## Wordpress configuration

Now you can access to you new Wordpress on on [localhost:8100](http://localhost:8100)

At the first start, WordPress will ask you for some information in order to connect to the database.

You must provide:

- database name : **wordpress**
- login : **wordpress**
- password : **wordpress**
- database adress : **db**
- table prefix : **wp_**

Send this informations and now enjoy your new installation !
