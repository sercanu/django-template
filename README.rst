========================
django-template
========================

This project is based on Django 1.5 TwoScoops Project (https://github.com/twoscoops/django-twoscoops-project). There are a few changes listed below:

#. Bootstrap 2 replaced with Bootstrap 3.
#. base.html adapted to Bootstrap 3.

Creating your project at local
==============================

We need a virtual environment. You can create with virtualenv or virtualenvwrapper::

    # with virtualenvwrapper
    $ mkvirtualenv dt
    # or with virtualenv
    $ virtualenv dt && source dt/bin/activate

Be sure that your virtual environment is activated.

Installation of Dependencies
----------------------------

In development::

    $ pip install -r requirements/local.txt

For production::

    $ pip install -r requirements.txt/production.txt

To create a new Django project called '**your_project_name**' using
django-template, run the following command::

    $ django-admin.py startproject --template=https://github.com/sercanu/django-template/archive/master.zip --extension=py,rst,html your_project_name
    # After creating project you can run it
    $ cd your_project_name
    $ python manage.py runserver
    # Now you can visit the main page.
    # syncdb for admin page
    $ python manage.py syncdb
    .....
    .....
    # After creating superuser account, you can login to /admin

