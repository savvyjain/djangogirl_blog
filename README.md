# Welcome to DJango Blog App

Clone the repository by the following command :
`$ git clone https://github.com/savvyjain/djangogirl_blog.git`

You should now be able to see the following directory structure:
```
.
└── dblog
    ├── blog
    │   ├── admin.py
    │   ├── apps.py
    │   ├── __init__.py
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── tests.py
    │   └── views.py
    ├── db.sqlite3
    ├── manage.py
    ├── mysite
    │   ├── __init__.py
    │   ├── settings.py
    │   ├── urls.py
    │   └── wsgi.py
    └── requirements.txt

4 directories, 15 files
```
## Create a new python environment 
`Linux` Assuming that you have Python 3+ installed, create the environment by typing in the following command: `$ python3 -m venv djangoenv` in your base directory.
Activate the environment by : `$ source djangoenv/bin/activate`
In case you want to deactivate the environment, simply type `$ deactivate`


### Install Requirements
To install the dependencies run the following commands
```
$ cd dblog/
$ python -m pip install --upgrade pip
$ pip install -r requirements.txt
```
### Create Databases
To create a database for our blog, let's run the following in the console: `$ python manage.py migrate` Default is `SQLite3`

To add our new model to our database, type `python manage.py makemigrations blog`

### Create Superuser
To log in, you need to create a _superuser_ - a user account that has control over everything on the site. Go back to the command line, type `python manage.py createsuperuser`, and press enter.
It must look something like
```
Username: ola
Email address: ola@example.com
Password:
Password (again):
Superuser created successfully.
```
### Launch and hands-on
To run the server: `python manage.py runserver`
To launch the application go to : [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)
Login with your super user credentials.

### References to learn some more Django
If you are new to programming and the above steps go tangent refer the Djangogirls tutorial at [https://tutorial.djangogirls.org/en/](https://tutorial.djangogirls.org/en/)

For Django Documentation go to : [https://www.djangoproject.com/](https://www.djangoproject.com/)

For more resources on Django go to : [https://github.com/wsvincent/awesome-django](https://github.com/wsvincent/awesome-django)
