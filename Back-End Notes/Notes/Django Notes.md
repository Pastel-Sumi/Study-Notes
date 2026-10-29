#Comandos 
* `workon`: Shows the list of virtual environments
* `workon environment_name`: Activates the virtual environment

We put the responsibility of loading the page to the client so the server can attend more clients, making this more scalable. (Considered one of the best practices)

* django-admin: To start a new project (utility that comes with django)
* django-admin startproject [projectname] . : Tells django to use the current directory as the project directory

As for the files inside our storefront subfolder:
- __init__.py: Defines the directory as a package.
- settings.py: Defines our application settings
- urls.py: We define the urls of our application.
- asgi.py / wsgi.py: Related to deployment.
- manage.py: This is a wrapper around Django admin

- `python manage.py runserver [PORT]`
- In Django each apps provides a certain functionality.
- `python manage.py startapp [appname` creates an app