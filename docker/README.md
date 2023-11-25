# common docker commands

docker pull centos
docker run -d -t --name myexample centos
docker exec -it myexample bash
docker stats 
docker stop
docker start
docker ps

# From YouTube video on how to create your own dockerfile/image/container

https://www.youtube.com/watch?v=SnSH8Ht3MIc&t=496s

docker build .
docker images
docker build -t hello-internet .
docker run -d -p 80:80 [image_id]
docker ps