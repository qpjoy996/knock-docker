docker run busybox echo hi there
docker run busybox ping google.com

docker system prune

docker create busybox echo hi there
docker start -a #ID
docker logs #ID

docker create busybox ping google.com
docker start #ID
docker logs #ID
docker stop/kill #ID


docker exec -it 
docker exec -i #ID redis-cli
docker exec -it #ID sh

docker run -d -p 5000:8080 qpjoy/nodeweb    (host-5000:inner-8080)


docker-compose up -d
docker-compose down


docker-compose up --build
docker-compose ps


docker build -f Dockerfile.dev .

docker run -p 3300:3000 #ID

docker run -p 3300:3000 -v /app/node_modules -v $(pwd):/app #ID

docker run -it #ID npm run test


docker attach #ID

docker run -p 8080:80 #ID


git remote add origin git@github.com:qpjoy/docker-react.git
git push origin master