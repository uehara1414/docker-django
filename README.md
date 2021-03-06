# docker-django
Docker template for static frontend and Django backend.

## Structure
Paths start with /api/ are redirected to the path of Django app and the others serve static files in /frontend directory.

## Setup
Create .env file
```
SECRET_KEY="secretkey"
VIRTUAL_HOST=foobar.net
DB_NAME=postgres
DB_USER=postgres
DB_PASS=postgres
DB_SERVICE=postgres
DB_PORT=5432
DEBUG=True
```

## Run
Run docker-compose up
```sh
docker-compose up -d
```

Then you can access frontend files from [http://localhost](http://localhost) and Django backend from [http://localhost/api/](http://localhost/api/)
