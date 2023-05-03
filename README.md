# Cinema API
API service for cinema management written on DRF

## Installing using GitHub
### Install PostgresSQL and create db
- git clone https://github.com/oksana0410/py-dockerize-drf-cinema.git
- cd cinema-API 
- `python -m venv venv` 
- source venv/bin/activate
- pip install -r requirements.txt
- `python manage.py migrate`
- `python manage.py runserver`

### Add the correct environment variables to your .env

- set POSTGRES_HOST=your_db_hostname
- set POSTGRES_DB=your_db_name
- set POSTGRES_USER=your_db_username
- set POSTGRES_PASSWORD=your_db_user_password
- set SECRET_KEY=your_secret_key

## Run with docker
### Docker should be installed

- docker-compose build
- docker-compose up

## Getting access
- create user via /api/user/register/
- get access token via /api/user/token/

## Features
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres and actors
- Creating Cinema halls
- Adding movies sessions
- Filtering movies and movie sessions
