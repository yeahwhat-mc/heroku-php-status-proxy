# heroku-php-status-proxy

Simple Heroku hosted PHP proxy to check the HTTP status of websites. The repository is based on Heroku's [php-getting-started](https://github.com/heroku/php-getting-started). It's purpose for [YEAHWHAT?!](http://yeahwh.at) is to allow requesting AJAX request without the proper "Access-Control-Allow-Origin" headers set. For more information, checkout our [fallback webserver](https://github.com/yeahwhat-mc/fallback-webserver).

## Running Locally

Make sure you have PHP, Apache and Composer installed.  Also, install the [Heroku Toolbelt](https://toolbelt.heroku.com/).

```sh
$ git clone https://github.com/yeahwhat-mc/heroku-php-status-proxy.git # or clone your own fork
$ cd php-status-proxy
$ composer update
$ foreman start web
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku open
```
