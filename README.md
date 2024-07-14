# poll-app-django

New postgresql container
$ docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres

First, after configuring the database in settings.py, run the following commands:
```bash
python manage.py migrate
```


After add a new model, run the following commands to create a new migration:
```bash
python manage.py makemigrations polls 
```
(polls is the name of the app)
If the migration is correct, run the following command to apply the migration:
```bash
python manage.py migrate
```


Run server:
$ python manage.py runserver
