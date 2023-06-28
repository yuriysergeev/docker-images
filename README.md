# docker-images

## busybnox with python app for testing
JFYI - docker commands:
    > docker run busybox echo "Hello world"
    > docker ps
    > docker ps -a 
    > docker images
    > docker images -a 
    > docker build -t busybox-python .
    > docker run -p 8080:8000 -d busybox-python:latest
    > docker logs <put_here_docker_id> -f
    > docker exec -it <put_here_docker_id> /bin/bash'
    > docker commit <put_here_docker_id> busybox-python:0.1
    > docker tag busybox-python:0.1 <dockerhub-name>/busybox-python:0.1
    > docker tag busybox-python:latest <dockerhub-name>/busybox-python:latest
    > docker login
    > docker push <dockerhub-name>/busybox-python:0.1
    > docker push <dockerhub-name>/busybox-python:latest
    > docker stop <put_here_docker_id>
    > docker rm <put_here_docker_id>
    > docker rmi busybox-python:0.1
    > docker rm -vf $(docker ps -a -q)
    > docker rmi -f $(docker images -a -q)
