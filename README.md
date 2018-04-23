# DjangoDocker

### Start project voor Django, Gunicorn, NGINX, Postgresql dmv Docker containers

#### Hoe te gebruiken

- clone de repo
- run docker-compose build
- run docker-compose up -d en ga naar http://localhost:8000 
- run docker exec -ti dg01 python /src/manage.py migrate
- run docker exec -ti dg01 python /src/manage.py createsuperuser

#### Te gebruiken commando's:

- **docker-compose build**              // build/rebuild de containers
- **docker-compose up -d**              // Start de oplossing, webserver start op localhost:8000
- **docker-compose down**               // Stop de oplossing

#### Shell toegang:

- **docker exec -ti ng01 bash**         // open bash shell in nginx container
- **docker-compose exec nginx bash**    // open bash shell in nginx container

- **docker exec -ti dg01 bash**         // open bash shell in web container
- **docker-compose exec web bash**      // open bash shell in web container

- **docker exec -ti ps01 bash**         // open bash shell in db container
- **docker-compose exec db bash**       // open bash shell in db container

#### Logfiles bekijken:

- **docker-compose logs nginx**         // Logfiles nginx container
- **docker-compose logs web**           // Logfiles web container
- **docker-compose logs db**            // Logfiles db container
