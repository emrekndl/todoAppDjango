## Todo App - Django
<br />
<p align="center">
<img src="images/todoAppDjango.png"  height="350" width="650" >
<br />
A simple todo app built with django - Posgresql Database and Docker Compose
</p>
<br />
<br />

## Setup

To get this repository, run the following commands inside your terminal.

```bash
$ git clone https://github.com/emrekndl/todoAppDjango.git
```
- *Note:* First you need to rename ".env.sample" file to ".env".

- For manuel installations (without docker compose).
```bash
$ python manage.py makemigrations
```

```bash
$ python manage.py migrate
```

```bash
$ python manage.py createsuperuser
```

```bash
$ python manage.py runserver
```

###### Runing with Docker Compose

- server and port: http://0.0.0.0:8001/
```bash
docker compose up
```
