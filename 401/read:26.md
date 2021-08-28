# # Read: Class 26 Intro to Django
- Django is a high-level Python web framework that enables rapid development of secure and maintainable websites
- Django is open source which means the code is available for free on github and can be downloaded onto developers computer and used.
- Django's oganization is managed by a non-profit.
- Django code is lead by a core team of volunteers

- Django helps you write software that is:

	1. Complete
	2. Versatile
	3. Secure
	4. Scalable
	5. Maintainable
	6. Portable	

- Django is somewhat opinionated.
- urls.py send the request to the right view
- views.py Handles the request and queries data
- models.py Defines data models
- HTML templates Renders data   

- The outer mysite/ root directory is a container for your project. Its name doesn’t matter to Django; you can rename it to anything you like.
- manage.py: A command-line utility that lets you interact with this Django project in various ways. You can read all the details about manage.py   in django-admin and manage.py.
- The inner mysite/ directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).
- mysite/__init__.py: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.
- mysite/settings.py: Settings/configuration for this Django project. Django settings will tell you all about how settings work.
- mysite/urls.py: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.
- mysite/asgi.py: An entry-point for ASGI-compatible web servers to serve your project. See How to deploy with ASGI for more details.
- mysite/wsgi.py: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

-Source from (https://docs.djangoproject.com/en/3.0/intro/tutorial01/)