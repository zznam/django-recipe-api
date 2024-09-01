# c2-recipe-app-api-2

Course code for: Build a Backend REST API with Python &amp; Django - Advanced: Take the course here: https://londonapp.dev/c2

## Commands

### Running Tests

```sh
docker-compose run --rm app sh -c "python manage.py test"
```

### Starting a New App

```sh
docker-compose run --rm app sh -c "python manage.py startapp core"
```

### Making Migrations

```sh
docker-compose run --rm app sh -c "python manage.py makemigrations"
```

### Waiting for DB and Migrating

```sh
docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"
```

### Running Tests and Linting

```sh
docker-compose run --rm app sh -c "python manage.py test && flake8"
```

### Managing Docker Volumes

```sh
<!-- List volumes: -->
docker volume ls
<!-- Remove volume: -->
docker volume rm django-recipe-api_dev-db-data
<!-- Stopping Containers -->
docker-compose down
```
