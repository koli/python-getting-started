# Python: Getting Started

A barebones Django app, which can easily be deployed to Koli.

## Running Locally

Make sure you have Python [installed properly](http://install.python-guide.org).  Also, install the Postgres.

```sh
$ git clone git@github.com:koli/python-getting-started.git
$ cd python-getting-started

$ pip install -r requirements.txt

$ createdb python_getting_started

$ python manage.py migrate
$ python manage.py collectstatic

$ gunicorn gettingstarted.wsgi --log-file -
```

Your app should now be running on [localhost:5000](http://localhost:5000/).