## Library Management System 

 Ensure you have the following on your PC:

- Python 3
- Pipenv
- Virtualenv (or virtualenvwrapper)
- Docker Desktop

### Install Python Modules

$ pipenv install flask flask-sqlalchemy flask-marshmallow marshmallow-sqlalchemy

$ pipenv install pylint-flask 

### Activate venv

$ pipenv shell

### Create DB by writing those command

$ python

>> from app import db

>> db.create_all()

>> exit()

### Run Server

>python app.py

#### Library.rar file is the Flask application without Docker

### Here is link of Test Documentation which is published by Postman

https://documenter.getpostman.com/view/10932897/SzYbxxCX?version=latest

### Containerize the solution with Docker

> Create "Dockerfile" on the project

> We have to specify the host as 0.0.0.0 in "app.py" file

> We can build our image with the docker build command :

>> docker build . -t library:v1

> Once the build process is done, we can run the application with the docker run command :

>> docker run -p 5000:5000 library:v1

#### Library folder is the final project
