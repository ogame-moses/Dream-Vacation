The Dream-Vacation-App is a full-stack web application that helps users explore vacation destinations
built with a React frontend, Node.js backend, PostgreSQL database, and fully containerized using Docker and Docker Compose.

Dream-Vacation-App
required packages are;  Install react, react-dom, react-scripts, axios

As regard this project we use docker-compose command to build and run both frontend and backend with the databbase together.
Note: frontend and backend can be built differently, also postgress is used for database

To build frontend,  use the command
# docker build . -t moses-frontend:latest 

You must run this command where the Dockerfile is located

To push this to docker hub, we need to tag our image
# docker build . -t ogame-moses/moses-frontend:latest

You can check your image by running
# docker images

To containarize your docker image, run # docker run -d -p 80:80 ogame-moses/moses-frontend:latest

Note wiskky is my docker hub username, change it to your own docker hub username.

Then run # docker ps



On your broswer, type http:localhost 

To push your image into docker hub, Then run

# docker push ogame-moses/ogame/kc-frontend:latest 

Login into your docker hhub accont and check 

NOTE For backend ollow the same step aove to run docker build command and push.

Using docker compose to containerize your application


To run your docker compose, use the below command # docker-compose up --build

After finish running, then check yyour image and the container  # docker images



You will notice that, two images are added dream-vacantion-backend and dream-vacantion-frontend.

Also, check if your container is running
# docker ps



Now go to your browser and check yyour application if it is running

http://localhost:3000
