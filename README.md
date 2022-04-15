# Docker Django Celery Redis

##

## Requirements

- Install [Docker](https://www.docker.com/) (preferabley with desktop app)
- Run `docker-compose build`
- Run `docker-compose up`
- Go to [http://127.0.0.1:8000](http://127.0.0.1:8000) to view the site

##

> Interactive Command Line Interface

- Run `docker exec -it container_name /bin/bash OR sh for alpine`
- Run `python3 manage.py migrate`.

##

<details>

<summary>
    <b>Optional</b>
</summary>

- To create a new django project. Run `docker-compose --rm app django-admin startproject project_name .` after executing build command.

- To test celery tasks follow these commands:
- After entering in the interactive command line interface run `python3 manage.py shell`
- Run `from new_app.tasks import add`
- Run `add.delay(4, 4)`

</details>

##
