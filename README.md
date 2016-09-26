# Relationship Repo

## Project Setup


### Install Symfony

``` javascript

  sudo curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
	sudo chmod a+x /usr/local/bin/symfony

```

### Pull the Project

``` javascript

cd localRepo
git pull origin master

```

### Install Composer

``` javascript

composer install

```
#### If you have the date time error
Open your php.ini file and change

``` javascript

:date.timezone =

```
to

``` javascript

date.timezome = "Europe/Amsterdam"

```

#### If you don't know which php.ini file is your working one

``` javascript

php --ini

```

## Start the server

``` javascript

app/console server:start

```
