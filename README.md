# Sample Docker Compose file with MySQL and PHPmyAdmin UI.

## How-to

1) Check that the ports 6033 and 8081 are not alread used otherwise, change the ports in the docker compose file

    $ docker ps

2) Start with:

    $ docker-compose up -d

3) Head to the main UI, go to http://localhost:8081/

4) Login with the credentials provided in the docker-compose.yml file

5) Import DB with the CLI

    $ docker exec -i container_id /usr/bin/mysql -udb_user -pdb_user_pass -hdb app_db < /path/to/my/file

## Credits

Author: Christian BELLET