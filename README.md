# Slim Boilerplate
A PHP boilerplate based on [Slim Framework](http://www.slimframework.com/), for start projects with [Eloquent ORM](https://laravel.com/docs/5.2/eloquent), Validation, Auth (JWT), Repositories and Transformers ready.

This boilerplate is written for RAD (Rapid Application Development).

Anyway it introduces some layer that will help you if the application will grow.
In this case i suggest you to drop Eloquent (or at least use only the query builder and use interfaces instead of Domain Model that extends Eloquent Model).

# Installation and Setup
You need [composer](http://getcomposer.org) and [git](https://git-scm.com/) for download and install the repository.

```shell
$ git clone https://github.com/damianopetrungaro/slim-boilerplate.git
$ php composer.phar install
```
Edit the `.env.example` to `.env` and override it with your credentials.
```shell
$ php vendor/bin/phinx migrate
```
#### Container
All the object into the container are setted into the `bootstrap/container.php` file

#### Info
The routes are into the `app/Routes`, you can add all the .php file you want, each file will be read by slim for catch all the routes.

The exception handler is overriden into the `bootstrap/container.php` file.
For more details, info or bugs, just open a  new issue to to [repository issue tracker](https://github.com/damianopetrungaro/slim-boilerplate/issues).


# Issue tracking
Please report any issues to [repository issue tracker](https://github.com/damianopetrungaro/slim-boilerplate/issues).
