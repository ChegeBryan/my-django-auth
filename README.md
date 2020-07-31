# My Django Auth

Tickering around with django extended user authentication

## Getting started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites

- python 3.8.2
- pip3

If you wish to clone the repo please satisfy the requirements in the requirements.txt

## Installing

```
clone the repo to local machine

git clone https://github.com/ChegeBryan/my-django-auth.git

pip3 install virtualenv

```

### Create a virtual environment and install requirements

- Navigate to the cloned repo directory and open terminal from there.
- run `virtualenv venv` to create virtual environment with the name `venv`
- activate the virtualenv by `source venv/bin/activate`
- `pip3 install -r requirements.txt` to install app requirements on your virtual environment

### Starting the server (development environment)

For the Social Auth to work on your local you will need the required OAuth Accounts for the specific Social Apps you are testing for.
For GitHub, set the following:

```
SOCIAL_AUTH_GITHUB_KEY
SOCIAL_AUTH_GITHUB_SECRET
```

while still at the terminal:

- run the migration `python manage.py migrate`
- Start the app by running `python manage.py runserver`
