# Heroku

## Basics

### Login
```bash
heroku login
```

### Create an heroku app
```bash
heroku create <appname>
```
### Clone an existing heroku app
```bash
heroku git:clone -a <appname>
```

### Add heroku remote into an repository
```bash
heroku git:remote -a <appname>
```

### Push to Heroku
```bash
git push heroku master
```

### Set Build packs
```bash
heroku buildpacks:set heroku/php
```

## Procfile

### Procfile : Set root folder
```
web: vendor/bin/heroku-php-apache2 public/
```

## ClearDB 

### Create CLear DB (ignite 5MB)

```bash
heroku addons:create cleardb:ignite
```

```php
<?php
$url = parse_url(getenv("CLEARDB_DATABASE_URL"));

$server = $url["host"];
$username = $url["user"];
$password = $url["pass"];
$db = substr($url["path"], 1);

$conn = new mysqli($server, $username, $password, $db);
?>
```

## Mongolab (496MB free)

```bash
heroku addons:create mongolab:sandbox
```

## Available Build Packs

| Language | Pack | Url |
| -------- | :---:| ---:|
| Ruby | heroku/ruby | [https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-ruby](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-ruby) |
| Node.js | heroku/nodejs | [https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-nodejs](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-nodejs)|
| PHP | heroku/php | [https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-php](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-php)|
| Python | heroku/python | [https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-python](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-python) |




