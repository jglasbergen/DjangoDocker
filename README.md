# DjangoDocker

### Start project voor Django, Gunicorn, NGINX, Postgresql dmv Docker containers

#### Hoe te gebruiken

- clone de repo
- run docker-compose build
- run docker exec -ti web python /src/manage.py createsuperuser
- run docker-compose up -d en ga naar http://localhost:8000 

#### Te gebruiken commando's:

- **docker-compose build**          // build/rebuild de containers
- **docker-compose up -d**          // Start de oplossing, webserver start op localhost:8000
- **docker-compose down**           // Stop de oplossing

#### Shell toegang:

- **docker exec -ti nginx bash**    // open bash shell in nginx container
- **docker exec -ti web bash**      // open bash shell in web container
- **docker exec -ti db bash**       // open bash shell in db container

#### Logfiles bekijken:

- **docker-compose logs nginx**     // Logfiles nginx container
- **docker-compose logs web**       // Logfiles web container
- **docker-compose logs db**        // Logfiles db container
