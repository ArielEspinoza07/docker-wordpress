# Simple docker for wordpress

## Configuration

### ENV
    
    create .env file from .env.example

    Mac/Linux
        cp .env.example .env

    Windows 
        copy .env.example .env

### NGINX

    go to .docker/nginx folder

    copy nginx.conf.example to wordpress.conf

### Wordpress Project

    put your project inside src folder and rename it to wordpress

#### if you don't want to rename it

    go to .docker/nginx/wordpress.conf 
    found root
    modify from /var/www/html/wordpress
    to /var/www/html/{project_folder_name}


### Build

    docker-compose build

####  without cache

    add ---no-cache

### Up

    docker-compose up -d