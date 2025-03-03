Workflows main.py have some secret key as like github user and passwd also aws pem key user and passswd

we set user password in setting on secrets and variable option . Now CICD and docker are working .

*** Manual setting ***

Go your ec2 and git clone from my flask-student-attend-Actionhub-app.
docker-compose up --build
docker-compose -f docker-compose.yml down
docker-compose up --build

**** We can push all image in docker hub ***

# Docker login 

 docker image tag flask-todo:latest ashis103/flask-todo:latest
 docker images
docker push ashis103/flask-todo
 docker image tag flask-student-attendance-app_app:latest ashis103/flask-student-attendance-app_app:latest
  docker images
  docker push ashis103/flask-student-attendance-app_app
