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

## Commands of Note


### Server Start

``` javascript

app/console server:start

```

### Create the Database

``` javascript

app/console doctrine:database:create

```

### Create an entity/model

``` javascript

app/console doctrine:generate:entity

```

### Generate CRUD

``` javascript

app/console doctrine:generate:crud

```

### Generate Table/Update the Schema

``` javascript

app/console doctrine:schema:update -force

```

## Project directories/files

### For Database

``` javascript

app/config/parameters.yml.dist
app/config/parameters.yml

```

### Views

``` javascript

app/Resources/views

```

### Base Twig Template is in

``` javascript

app/Resources/views

```

### Base Home Page is in

``` javascript

app/Resources/views/default

```
