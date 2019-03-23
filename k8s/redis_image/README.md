docker build .
docker run #ID


docker build -t qpjoy/redis:latest .
docker run qpjoy/redis


one cmd:
docker run -it alpine /bin/bash
another cmd:
docker commit -c 'CMD ["redis-server"]'

docker run #ID