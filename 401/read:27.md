# Read: Class 27 Django Models

## Using Models
- **Models** are used to access and manage data through python objects in django web applications.
- **Models** Define the structure of stored data.
- You don't need to talk to a database once you have chosen which one you want to use, 
	just write write the model structure and other code, and django will handle communicating with the database for you.

- Once you have decided on your models and field, you need to think about the relationships. 
	Django allows you to define relationships that are 
	1. One to one (OneToOneField), 
	2. One to many (ForeignKey)
	3. Many to many (ManyToManyField).

- **Models** are usually defined in an application's models.py file. 
	They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.
	- Source from (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- A **model** can have an arbitrary number of fields, of any type — each one represents a column of data that we want to 
	store in one of our database tables. Each database record (row) will consist of one of each field value.
	- Source from (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- A **model** can also have methods.
- Almost every model needs a __str__ method that returns a human readable string for each object.
- Once you've defined your model classes you can use them to create, update, or delete records, 
	and to run queries to get all records or particular subsets of records
	- Source from (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- To create a record you can define an instance of the model and then call save().
- You can search for records that match certain criteria using the model's objects attribute.

## Django Admin
- The Django admin application can use your models to automatically build a site area that you can use to 
	create, view, update, and delete records.
	- This can save you a lot of time during development, making it very easy to test your models and get a feel 
		for whether you have the right data. 
- In order to log into the admin site, we need a user account with Staff status enabled.
- In order to view and create records you also need this user to have permissions to manage all our objects.
- python3 manage.py createsuperuser (to create a super user).
- python3 manage.py runserver (to run the server).
    - Source from (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)