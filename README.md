##PITCH
##Description
A pastebin or text storage site is a type of online content hosting service where users can store plain text, e.g. to source code snippets for code review via Internet Relay Chat. This application allows users to paste their code and share it with others for code review.

Link to deployed site


Table of content
Description
API endpoints
Setup and installations
Deployment
Contributing
Bugs
Contact me
Licensing
endpoints
API Endpoint	Description	Request
http://pasteb1n.herokuapp.com/snippets/	Display a JSON object containing all snippets	GET
http://pasteb1n.herokuapp.com/snippets/	Create a new snippet	POST
http://pasteb1n.herokuapp.com/snippet/1/	Display a JSON object of a specific snippet	GET
http://pasteb1n.herokuapp.com/snippet/1/	Edit a snippet	PUT
http://pasteb1n.herokuapp.com/snippet/1/	Delete a snippet	DELETE
Setup and installations
Prerequisites
Python3.6
Postgres
virtualenv
Pip
Django
Django Rest Framework
Technologies used
- Python 3.6
- HTML
- Bootstrap 4
- Heroku
- Postgresql
- Django, Django Rest Framework
Clone the Repo and checkout into the project folder.
git clone git@github.com:newtonkiragu/django-restful.git && cd django-restful
Create and activate the virtual environment
python3.6 -m virtualenv virtual
source virtual/bin/activate
Setting up environment variables
Create a .env file and paste paste the following filling where appropriate:

SECRET_KEY='<Secret_key>'
NAME='tutorial'
USER='<Username>'
PASSWORD='<password>'
HOST='localhost'
MODE='dev'
DEBUG=True
DISABLE_COLLECTSTATIC=1
Install dependancies
Install dependancies that will create an environment for the app to run pip install -r requirements.txt

Create the Database
In a new terminal, open the postgresql shell with psql.

CREATE DATABASE tutorial;
Make and run migrations
python3.6 manage.py makemigrations && python3.6 manage.py migrate
Run the app
python3.6 manage.py runserver
Open localhost:8000

Deployment
To deploy the application, please follow the instructions in this gist

Contributing
Please read this comprehensive guide on how to contribute. Pull requests are welcome :-)

Bugs
Create an issue mentioning the bug you have found

Known bugs
none yet
Feature request
Create an issue mentioning the feature you would like implemented

Support and contact details
Contact Newton Karanu for further help/support

License
MIT

Copyright (c)2018 Newton Karanu