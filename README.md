# login-app-docker
docker setup to run needed applications for login-app

## basic commands for instant quick use
### docker commands
***
#### to enter into a container
> docker exec -it <container_name> bash

### mysql commands
***
#### to enter into mysql database (even if you are inside a conatiner)
> mysql -u <user_name> -p <database_name>
#### to list all tables
> show tables;

## extra notes
the reason for using *docker-entrypoint-initdb.d* directory in mysql container is because of the style of code given in the below link which will execute all the sql files in that directory when container is started
https://stackoverflow.com/questions/38713597/create-table-in-postgresql-docker-image/38714511#38714511
