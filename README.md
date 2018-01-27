# angular-docker-nginx
An example of how to install and run an Angular application locally and deploy it to a Docker image with nginx.
>This example uses node v8, the latest angular cli version, the latest docker community edition version and the latest nginx version for theoretical purposes.
(01/26/2018)
### Installation
This application requires:
-   [Node.js](https://nodejs.org/) to run locally.
-   [Angular CLI](https://github.com/angular/angular-cli) to use Angular commands.
-   [Docker](https://www.docker.com/) CE to build and run virtual images.
### Run locally
Inside angular-docker-nginx run:
```sh
$ ng serve
```
This service will run in localhost:4200 and will be synchronized every time a file is saved.
### Deploy with Docker
Inside angular-docker-nginx build the docker image:
```sh
$ sudo docker build -t angular-docker-nginx .
```
In order to run the latest version of the images run:
```sh
$ sudo docker run -i -t -p 8080:80 angular-docker-nginx:latest
```
License
----
MIT
