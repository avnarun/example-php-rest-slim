# example-php-rest-slim
The purpose of this project is to create a very simple localhost rest api server and then ability to call those rest apis via any client.

This would be useful for anyone new to rest api concepts and will help to understand different HTTP methods and how to marry them to appropriate CRUD operations.

This is built php SLIM framework. Also, I have taken basic code from https://github.com/ccoenraets/wine-cellar-php

#Installation of Rest API Server
You can clone this git repository to your local, I will recommend to clone it under your www folder
git clone https://github.com/avnarun/example-php-rest-slim.git

cd to the working directory
cd example-php-rest-slim

Install composer dependencies, includes slim framework
composer install

All done

#Usage (doing CRUD operation from a rest api client)
You can use any rest api client you have and can do basic CRUD operations

Database record RETRIEVAL (performed via HTTP GET)
http://localhost/example-php-rest-slim/wines
http://localhost/example-php-rest-slim/wines/1 (:id)
http://localhost/example-php-rest-slim/wines/search/:query

Database record CREATE (performed via HTTP POST)
http://localhost/example-php-rest-slim/wines

Database record UPDATE (performed via HTTP PUT)
http://localhost/example-php-rest-slim/wines/1 (:id)

Database record DELETE (performed via HTTP DELETE)
http://localhost/example-php-rest-slim/wines/1 (:id)
