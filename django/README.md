1. Create new project
```python
# Will create directory "your-website-name"
django-admin startproject your-website-name
```
```shell
# Directory structure
website/
    manage.py
    website/
        __init__.py
        settings.py
        urls.py
        wsgi.py
```
2. Create a new app
```python
# Will create directory "your-app" in your project directory
python manage.py startapp your-app

# Linux with python 2 and python3 installed
python3 manage.py startapp your-app
```
```shell
# Directory structure
your-app/
    __init__.py
    admin.py
    apps.py
    migrations/
        __init__.py
    models.py
    tests.py
    views.py
```
3. Run server: 
```python
python manage.py runserver

# Linux with python 2 and python3 installed
python3 manage.py runserver
```
