# bootstrap-postgres 
- Create Dockerfile
- Generate table and data sql
- Create tables and data
- Cretaes docker image

## docker exec
docker pull postgres:latest
docker volume create postgres-volume
docker run -d --name=my-postgres -p 5432:5432 -v postgres-volume:/var/lib/postgresql/data -e POSTGRES_PASSWORD=[your_password] postgres
docker logs my-postgres
docker exec -it my-postgres psql -U postgres