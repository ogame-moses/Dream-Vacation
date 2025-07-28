The Dream-Vacation-App is a full-stack web application that helps users explore vacation destinations
built with a React frontend, Node.js backend, PostgreSQL database, and fully containerized using Docker and Docker Compose.

Dream-Vacation-App
required packages are;  Install react, react-dom, react-scripts, axios

As regard this project we use docker-compose command to build and run both frontend and backend with the databbase together.
Note: frontend and backend can be built differently, also postgress is used for database

To build frontend,  use the command
# docker build . -t ogame/kc-frontend:latest 
<img width="1340" height="226" alt="frontend-" src="https://github.com/user-attachments/assets/7b75ed36-1ff9-41ef-bdcb-9dd8fdfe2538" />

You must run this command where the Dockerfile is located

To build backend,  use the command
# docker build . -t ogame/kc-backend:latest
<img width="1326" height="157" alt="backeend-" src="https://github.com/user-attachments/assets/c5395719-2797-4a35-b35d-3ca742e5149a" />


To containarize your docker image, run 
# docker run -d -p 80:80 ogame-moses/moses-frontend:latest
# docker run -d -p 3000:3000 ogame-moses/moses-backend:latest
Note moxis07 is my docker hub username, change it to your own docker hub username.

Then run # docker ps

On your broswer, type http:localhost 

To push your image into docker hub, Then run

# docker push ogame-moses/ogame/kc-frontend:latest 

Login into your docker hub accont and check 
<img width="1294" height="284" alt="image" src="https://github.com/user-attachments/assets/8e9b8f57-6b70-4d2a-af2f-106f4cbb8a5e" />

NOTE  the same step above is repeated for the backend ;to run docker build command and push.

Using docker compose to containerize your application


To run your docker compose, use the below command # docker-compose up --build
<img width="1535" height="366" alt="image" src="https://github.com/user-attachments/assets/e37978cd-c9cf-48b6-b503-e3d8b57b6cfb" />

After finish running, then check yyour image and the container  # docker images

You will notice that, two images are added dream-vacantion-backend and dream-vacantion-frontend.

Also, check if your container is running
# docker ps



Now go to your browser and check yyour application if it is running

http://localhost:3000
