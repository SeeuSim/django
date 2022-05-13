=====
Polls
=====

Polls is a Django app to conduct web-based polls. For each question,
visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Basic setup
-----------
1. Create a directory to host your project.

2. Check your django version by running:

   ``python -m django --version``
   
   If not installed, install django.

3. Run this command to initialise the project:

   ``django-admin startapp <project_name_here>``
   
4. Download this project.

5. Change directory to ''polls-django/dist''.

6. Run this command:

   ``python -m pip install --user polls-django-0.1.tar.gz``
   
Quick start
-----------

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('polls/', include('polls.urls')),

3. Run ``python manage.py migrate`` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.
