# django_email_user

A simple django app to override the User model removing the username and requiring an email instead.

Also sends an email everytime a user signs up.

Installation:

Add to your apps:
'users',

Add to settings.py:
AUTH_USER_MODEL = 'users.User'
MAILING_LIST = ['you@yourserver.com']

python manage.py migrate

WARNING - Exisiting users will be destroyed.
