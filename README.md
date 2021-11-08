# Setup Oracle Database with Docker
## Install
1. Go to the official [Oracle Image on Docker Hub](https://hub.docker.com/_/oracle-database-enterprise-edition)
2. Login to your Docker account
3. Click proceed to checkout
4. Enter your data and accept all Oracle terms of service
5. Close the browser and switch to shell
6. Make sure Docker is running
7. `docker login`
8. Run Container:
```
docker run --cpus 1 --memory 1g -p 1521:1521 --name oracle-db store/oracle/database-enterprise:12.2.0.1
```
9. Wait until DB started
10. DB is running!

**Warning:** If you remove the Docker container your DB content is gone. You can prevent this by mapping a volume. Or you just don't remove the container :)

## Default credentials:
```
Hostname: localhost
Port: 1521
SID: ORCLCDB
User: sys as sysdba
Password: Oradoc_db1
```