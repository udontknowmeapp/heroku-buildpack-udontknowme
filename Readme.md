# Heroku buildpack: udontknowme

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for `udontknowme`


Usage
-----

Example usage:

    $ ls
    Procfile  requirements.txt  frontend/package.json webapp/app.py

    $ heroku create --buildpack git://github.com/udontknowmeapp/heroku-buildpack-udontknowme.git

    $ git push heroku master
    ...
    -----> Python app detected
    -----> Installing runtime (python-2.7.10)
    -----> Installing dependencies using pip
           Downloading/unpacking requests (from -r requirements.txt (line 1))
           Installing collected packages: requests
           Successfully installed requests
           Cleaning up...
    -----> Discovering process types
           Procfile declares types -> (none)

You can also add it to upcoming builds of an existing application:

    $ heroku buildpacks:set it://github.com/udontknowmeapp/heroku-buildpack-udontknowme.git
