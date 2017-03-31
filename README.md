# Music History API for Onodric

A front end developed in AngularJS supplied to the developers at Nowhere. Used to expose relevant API resources for view, creation, editing, or deletion of music library members in a user-friendly way.

## Steps to Install

The API uses the Django framework, running on Python 3.6

#### To install the project locally:
1. Start the API component:
  1. download or clone the [Music History Django API](https://github.com/Onodric/django-music-history)
  1. Set up [Python 3.6](https://www.python.org/) on your machine per the install instructions
  1. Install [pip](https://pip.pypa.io/en/stable/installing/)
  1. Install Django 1.10.5 via pip: `pip install django`
  1. Clone the repository to desired location
  1. Migrate the database tables. In the main project directory `~/Music_History/music_history_api` (where `manage.py` is located), run the command `python manage.py migrate`
  1. Create a superuser for testing purposes: `python manage.py createsuperuser`.
  1. Start the development server. Run the command `python manage.py runserver`. Take note of the IP address and host port given.

1. Start the front end component ([_This_ repo[https://github.com/Onodric/angular-music-history]]), by running a local server (such as http-server) from the directory containing `index.html`. *Note: the port for the API and the port for the front-end MUST BE DIFFERENT. By default, they are!* 
1. Start a browser, and navigate to the correct IP and port,  followed by `/api/`. i.e. ```127.0.0.1:8000/api/```. Other resources may be reached from `admin` and `api_auth`.
  - Defaults follow:
    - [Api Root](http://localhost:8080)
    - [Admin Root](http://localhost:8000/admin)

## Installed Dependencies 

The API relies upon the following dependencies:

1. Python >v.3.6
1. Django >v1.10.5

## System Config

The API should run on all systems that meet the dependency requirements.
