## Flask Todo App using SQLAlchemy and SQLite database.
Tutorial link: https://www.python-engineer.com/posts/flask-todo-app/

### Setup
Create project with virtual environment

```console
$ mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

Activate it
```console
$ . venv/bin/activate
```

or on Windows
```console
venv\Scripts\activate
```

Install Flask
```console
$ pip install Flask
$ pip install Flask-SQLAlchemy
```

Set environment variables in terminal
```console
$ export FLASK_APP=app.py
$ export FLASK_ENV=development
```

or on Windows
```console
$ set FLASK_APP=app.py
$ set FLASK_ENV=development
```

Setup initial database by running python interactive shell using `python`, then
```
from app import db, app
with app.app_context():
    db.create_all()
```

Run the app
```console
$ flask run
```
