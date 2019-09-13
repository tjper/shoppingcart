# shoppingcart

This application was build as part of a technical exercise for Artifiact
Uprising. The application is broken up into three services: web, server, and
database. All services run as a docker containers.

Therefore, application requires docker be installed on the system in order to
run all the services.

Follow these steps to being running the application:
1. navigate to this repos base directory
2. execute snippet below in your terminal

```bash
  make app
```

3. open localhost:3000 in your browser

If you have any issues, make sure the ports utilized by theses services are not
conflicting with other processes.

Ports: 8080, 3000, 3306
