# Install WordPress | MariaDB | Nginx with Docker Compose

With this project you can quickly run the following:
- [WordPress](https://hub.docker.com/_/wordpress)
- [MariaDB](https://hub.docker.com/_/mariadb)
- [Nginx](https://hub.docker.com/_/nginx)

## Requirement and Installation

Make sure you have the latest versions of **Docker** and **Docker Compose** installed on your machine. Then follow this:

1. Clone this repository
2. Copy and rename the example files:
    ```
    cp .env.db.example .env.db
    cp .env.wp.example .env.wp
    ```
3. Edit the newly created .env.db and .env.wp files with your specific values:
    - Open each file
    - Replace placeholder values with secure, unique passwords
    - Ensure database credentials match between the two files
4. Open a terminal and `cd` to the folder in which `docker-compose.yml` is saved and run:
    ```
    docker-compose up
    ```


## Usage

### Starting containers

You can start the containers with the `up` command in daemon mode (by adding `-d` as an argument) or by using the `start` command:

```
docker-compose up -d
```

### Stopping containers

```
docker-compose stop
```

### Removing containers

To stop and remove all the containers use the`down` command:

```
docker-compose down
```

Use `-v` if you need to remove the database volume which is used to persist the database:

```
docker-compose down -v
```

# Disclaimer

This is part of my learning process in understanding Docker and Docker Compose. For local development only (not designed for production purposes). Thx! :)