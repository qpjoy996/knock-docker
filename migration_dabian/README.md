# docker-compose
> 1. wget "https://github.com/docker/compose/releases/download/1.4.2/docker-compose-Linux-x86_64 > docker-compose"
     || curl -L 'url'
> 2. chmod +x docker-compose
> 3. mv docker-compose /usr/local/bin

# docker
> 1. apt.dockerproject.org
> 2. http://apt.dockerproject.org/repo/pool/main/d/docker-engine/

> 1. yum install yum-utils device-mapper-persistent-data lvm2
> 2. yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
> 3. yum --showduplicates list docker-ce | expand
> 4. yum install docker-ce-18.06.1.ce-3.el7.centos
> 5. usermod -aG docker kevin (non-root)

# docker command
> 1. docker run --rm busybox:latest /bin/echo "hello world"
> 2. docker run -it --rm busybox:latest
> 3. docker images
> 4. docker rmi 