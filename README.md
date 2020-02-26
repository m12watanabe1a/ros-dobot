# docker-ros-melodic

## Install

### Setup Repository
```
 $ git clone --recursive https://github.com/m12watanabe1a/docker-ros-melodic.git
 $ cd docker-ros-melodic
 $ docker-compose build
```

### Setup Docker-Machine for Mac
See https://qiita.com/shungok/items/6c5a7b5a9d63d51e6615

## Start up Docker countainer
execute ```setup.sh``` for docker hypervisor.
```
 $ ./setup.sh
 $ docker-compose up -d
```

## Login to The Container
```
 $docker exec -it roscore bash
```
