=====
Poll
=====

Polls is a Django app to conduct Web-based polls. For each question,
visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "polls" , "cities", "admin" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
        'cities',
        'pages'

    ]

2. Include the polls URLconf in your project urls.py like this::

    path('', include('pages.urls')),
    path('polls/', include('polls.urls')),
    path('admin/', admin.site.urls),
    path('cities/', include('cities.urls')),
    path('api/polls/', include('polls.urls')),
    path('api-auth/', include('rest_framework.urls'))

3. Run ``python manage.py migrate`` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.

5. Visit http://127.0.0.1:8000/cities/ to read more about the cities.