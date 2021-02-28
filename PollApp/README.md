# Polling App for Finnish Cities

> Python Django app to poll on Favourite City in Finland

## Quick Start

```bash
# Install dependencies
pipenv install

cd pollApp/pollster

# create a user 
python manage.py createsuperuser 

# login to admin area and add desired questions
localhost:8000/admin 




# Serve on localhost:8000
python manage.py runserver
```
Endpoints
```

localhost:8000
localhost:8000/cities
localhost:8000/polls


```

Running as a python package on a skeleton Django App

```
- Follow instructions on README.rst
- add include to "from django.urls import  path" as "from django.urls import include, path"
- cd pollApp
# install the package with 
- python -m pip install  django_polls_for_cities-0.1-py3-none-any.whl
- - run your skeleton App
```



