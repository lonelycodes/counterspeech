# Fancy Over-Engineered Go React App  (tm) 
This app is still in developent, enjoy with care!
At this point, it's not even clear what it should do.


## Getting started:
* download [docker-compose](https://docs.docker.com/compose/install/) if not already installed
Run the following commands:

```bash
$ docker-compose up
```
The React frontend is available at localhost:3000 and the RESTful go API at localhost:5000

Changing any frontend code locally will cause a hot-reload in the browser with 
updates and changing any backend code locally will also automatically update any changes.

Then to build prod images run:
```bash
$ docker build ./api --build-arg app_env=prod 
$ docker build ./frontend --build-arg app_env=prod
$ docker build ./db
```