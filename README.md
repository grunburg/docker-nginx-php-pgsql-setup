# docker-nginx-php-pgsql-setup
Docker, for **Larvel** made, web-server based on **[NGINX](https://hub.docker.com/_/nginx)**, **[PHP](https://hub.docker.com/_/php)** and **[Postgresql](https://hub.docker.com/_/postgres)**.

> **Attention**: If you don't want to use any database services, check out my other [Docker setup](https://hub.docker.com/_/php) or just remove Postgresql from [docker-compose](https://github.com/grunburg/docker-nginx-php-pgsql-setup/blob/master/docker-compose.yml) file.

### Installation

1. Clone this repository in your project folder.
```
$ git clone https://github.com/grunburg/docker-nginx-php-pgsql-setup .
```
2. Edit [default.conf](https://github.com/grunburg/docker-nginx-php-pgsql-setup/blob/master/default.conf) and [docker-compose.yml](https://github.com/grunburg/docker-nginx-php-pgsql-setup/blob/master/docker-compose.yml): ports, volumes, etc.

3. Install Laravel

4. To start the server, navigate to your folder via Terminal and run this command:
```
$ docker-compose up -d --build
```

> If this command doesn't work (especialy for **WSL** users), try to add **sudo** before the command.

5. Congratulations! You have succesfully setup **Docker** web-server for Laravel.

### Usage
* You can access your web server via browser [localhost:8000](http:localhost:8000) (Or your port that you configured earlier).
* To turn on your container or restart or stop it, you can now use **Docker Desktop** interface.

![Screenshot](https://i.ibb.co/3cW0d6r/image.png)

>In this example I'm running Laravel API on this Docker web-server.
