# shoppingcart

## Running the app

This application was build as part of a technical exercise for Artifiact
Uprising. The application is broken up into three services: web, server, and
database. All services run as docker containers.

Therefore, application requires docker be installed on the system in order to
run all the services.

Follow these steps to being running the application:
1. clone this repo via the code snippet below
> git clone --recurse-submodules https://github.com/tjper/shoppingcart

2. navigate to this repos base directory
3. run snippet below in your terminal
>  make app

4. open localhost:3000 in your browser

If you have any issues, make sure the ports utilized by theses services are not
conflicting with other processes.

Ports: 8080, 3000, 3306

## Stack

The backend server is written completely in Go. I utilized the Viper, Cobra,
and Chi packages with the intent on showing the effort I put into to making
applications easy to configure and modular. There are some integrations tests
in the server/testing directory. Theses tests are "golden" tests, which is a
testing technique that's compares the results of a test to the previous result
in order to ensure return values are not changing unexpectedly.

The database is a MySQL instance. While I am more comfortable with Postgres, I
wanted to dabble in MySQL given the small scope of this application, it's
gaining popularity, and it's utilization at Artifact Uprising.

The web application is a React Redux application.
