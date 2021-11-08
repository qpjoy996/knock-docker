### https://digitalavenue.dev/Run-Jenkins-On-Docker-Compose/
1. docker-compose --version
2. docker network create jenkins-net
3. docker volume create jenkins-docker-data
4. docker container run --name jenkins-server --detach --restart unless-stopped --network jenkins-net --hostname jenkins --publish 8080:8080 --volume jenkins-data:/var/jenkins_home jenkins/jenkins:lts
5. docker container ps
> 查看初始密码
6. docker exec jenkins-server cat /var/jenkins_home/secrets/initialAdminPassword