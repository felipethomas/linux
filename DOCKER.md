# instalação do Docker
1) seguir os passos em https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#set-up-the-repository

# comandos docker
1) docker --help
2) sudo docker container run hello-world
3) sudo docker container run debian bash --version
4) sudo docker container ps
5) sudo docker container ps -a
6) sudo docker container run --rm debian bash --version
7) sudo docker container run -it debian bash
8) sudo docker container run --name mydeb -it debian bash
9) sudo docker container ls
10) sudo docker container ls -a
11) sudo docker container start -ai mydeb
12) sudo docker container run -p 8080:80 nginx
13) sudo docker container run -p 8080:80 -v $(pwd)/html:/usr/share/nginx/html nginx
14) sudo docker container run -d --name ex-daemon-basic -p 8080:80 -v $(pwd)/html:/usr/share/nginx/html nginx

