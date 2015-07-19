# example-php-rest-slim
The purpose of this project is to create a very simple localhost rest api server and then ability to call those rest apis via any client.

This would be useful for anyone new to rest api concepts and will help to understand different HTTP methods and how to marry them to appropriate CRUD operations.

This is built php SLIM framework. Also, I have taken basic code from https://github.com/ccoenraets/wine-cellar-php

#Installation of Rest API Server

You can clone this git repository to your local, I will recommend to clone it under your www folder:-
```
git clone https://github.com/avnarun/example-php-rest-slim.git
```

cd to the working directory:-
```
cd example-php-rest-slim
```

Install composer dependencies, includes slim framework:-
```
composer install
```

Create database and create wine table using cellar.sql

Finally update database.php to reflect your db information

<b>All done and you should be ready to start making rest api calls !!!</b>

#Usage (doing CRUD operation from a rest api client)
You can use any rest api client you have and can do basic CRUD operations

<h4>Database record RETRIEVAL (performed via HTTP GET)</h4>
<a href="http://localhost/example-php-rest-slim/wines">http://localhost/example-php-rest-slim/wines</a>
<br/><a href="http://localhost/example-php-rest-slim/wines/1">http://localhost/example-php-rest-slim/wines/1</a> (:id)
<br/><a href="http://localhost/example-php-rest-slim/wines/search/CHATEAU">http://localhost/example-php-rest-slim/wines/search/CHATEAU</a> :query

<h4>Database record CREATE (performed via HTTP POST)</h4>
<a href="http://localhost/example-php-rest-slim/wines">http://localhost/example-php-rest-slim/wines</a>

<h4>Database record UPDATE (performed via HTTP PUT)</h4>
<a href="http://localhost/example-php-rest-slim/wines/1">http://localhost/example-php-rest-slim/wines/1</a> (:id)

<h4>Database record DELETE (performed via HTTP DELETE)</h4>
<a href="http://localhost/example-php-rest-slim/wines/1">http://localhost/example-php-rest-slim/wines/1</a> (:id)
