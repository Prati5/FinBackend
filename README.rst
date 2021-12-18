============
Installation
============

--------------
Pre-Requisites
--------------
* `Pycharm`
* `Ubntu/Windows`
* `Python3.9`
* `SQLite`
* `Virtual environment`




Installing the Project
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

::
    1. Create the virtual environments using python -m venv environment_name
    2. Install the required packages mentioned in the requirements folder
       pip install -r requirements/requirements.txt


Django Specific configurations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Populate DB using below commands:
    a. python manage.py makemigrations
    b. python manage.py migrate
2. Start server using below command:
    a. python manage.py runserver


----------------
Create superuser
----------------

Create a superuser or access the Django management shell.
    a. python manage.py runserver
    b. start server again and access django admin using below url:
    c. http://127.0.0.1/admin/login/?next=/admin/
    d. provide username/password and access Django admin
    e. create one group name "users" using below url:
       http://127.0.0.1/admin/auth/group/
    f. configure oauth app using below url:
       http://127.0.0.1/admin/oauth2_provider/application/add/
       if required please refer below url:
       http://django-oauth-toolkit.readthedocs.io/en/latest/rest-framework/getting_started.html#

Note:
~~~~~~~~~~~~~~~

    1. To avoid commit python compiled files(.pyc) files please add these into .gitignore file \*.pyc
    2. Before commit the code please use pep8 check. please refer below url:
        https://www.python.org/dev/peps/pep-0008/
            we can use PyCharm(editor) Code -> Inspect Code utility for pep8 guideline.


