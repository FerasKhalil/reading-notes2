# Read: Class 29 Django Custom User
## Django Custum User Model

- Setup
- To start, create a new Django project from the command line. We need to do several things:
1. create and navigate into a dedicated directory called accounts for our code
2. install Django
3. make a new Django project called config
4. make a new app accounts
5. start the local web server
- Here are the commands to run:
- $ cd ~/Desktop
- $ mkdir accounts && cd accounts
- $ pipenv install django~=3.1.0
- $ pipenv shell
- (accounts) $ django-admin.py startproject config .
- (accounts) $ python manage.py startapp accounts

	- Source from (https://learndjango.com/tutorials/django-custom-user-model)

- There are two  modern ways to create a custom user model in django:
	1. AbstractUser
	2. AbstractBaseUSer

- To create Superuser :
	- $ python manage.py createsuperuser

## DjangoX

🚀 Features
- Django 3.1 & Python 3.8
- Install via Pip, Pipenv, or Docker
- User log in/out, sign up, password reset via django-allauth
- Static files configured with Whitenoise
- Styling with Bootstrap v4
- Debugging with django-debug-toolbar
- DRY forms with django-crispy-forms

	- source from (https://github.com/wsvincent/djangox)