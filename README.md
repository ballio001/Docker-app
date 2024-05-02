# Docker how to use:
Have npm installed and express

Server just returns: a string for now. this was made to get used to using docker.

## how to run it as following:

open terminal where the file "dockerfile" is located.

run docker build -t node-app:1.0 . (runs docker with the app name/version in the current file location)

and to run it as localhost run:  docker run -d -p 3000:3000 node-app:1.0 with the localhost port 3000 (can be adjusted as needed)


## some functionalities in cmd:

``docker ps => shows current active containers.``

``docker ps -a => shows hidden containers.``

``docker logs => shows logs of active containers.``

for example: to Create an existing docker using nginx found on [docker hub ](https://hub.docker.com/).
we use the version of nginx, and give it a localhost port so we can use that domain to call for nginx.
We can also give it a name we do that by using:
``docker run --name [name] -d -p [localhostport]:[portofdocker] [dockername]:[version] `` 

for this example: `` docker run --name web-app -d -p 9000:80 nginx:1.25 ``

This will createe a docker container for nginx version 1.25, with the name web-app locally.

see [[docker hub nginx ](https://hub.docker.com/_/nginx)] for more information.
