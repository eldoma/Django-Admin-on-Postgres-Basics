# Django-Admin-on-Postgres-Basics

## Start local Postgres server in VS Code or IBM Cloud
### Once PostgreSQL is started, check the server connection information in the terminal. Need to save the connection information such as generated username, password, and host, etc, which will be used to configure Django app to connect to this database.

- pip install --upgrade distro-info
- pip3 install --upgrade pip==23.2.1 replace with python -m pip install --upgrade pip==23.3.1 --user

- pip install Django

### Install the Psyopg adapter:
- python -m pip install psycopg2-binary==2.9.7 --user

### Obtain the Code
wget -O Downloads/lab2_template.zip "https:____/IBM-CD0251EN-SkillsNetwork/labs/m4_django_app/lab2_template.zip"

### Go to specific Project directory
- cd lab2_template
- pip install virtualenv        
- virtualenv djangoenv replace with python -m venv djangoenv       
- source djangoenv/bin/activate replace with .\djangoenv\Scripts\activate    
- pip install -r requirements.txt

### Perform Migrations to create Necessary Tables

- python manage.py makemigrations    
- python manage.py migrate

# Test the Django connection
http://127.0.0.1:8000
![Django](https://github.com/eldoma/Django-Admin-on-Postgres-Basics/blob/main/Django%20test.jpg)

### Run this command to create a new superuser:
- python manage.py createsuperuser
- python manage.py runserver

## Launch the application on /admin
http://127.0.0.1:8000/admin
Should be showing this Admin page
![Admin](https://github.com/eldoma/Django-Admin-on-Postgres-Basics/blob/main/Django%20Admin.jpg)
