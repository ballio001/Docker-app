Docker how to use:
Have npm installed and express

Server just returns: "Welcome to my awesome app!"

how to run it as following:

open terminal where the file "dockerfile" is located.

run docker build -t node-app:1.0 . (runs docker with the app name/version in the current file location)

and to run it as localhost run:  docker run -d -p 3000:3000 node-app:1.0 with the localhost port 3000 (can be adjusted as needed)
