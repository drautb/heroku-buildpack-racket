Heroku buildpack: Racket
========================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for Racket apps.
It uses [Racket](http://racket-lang.org).

Usage
-----

Example usage:

    $ ls
    Procfile server.rkt

    $ heroku create --stack cedar --buildpack http://github.com/drautb/heroku-buildpack-racket.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> Racket Framework app detected
    -----> Building Racket Runtime Environment
    ...

The buildpack will detect that your app has a `server.rkt` in the root.
