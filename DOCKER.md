# My Docker CHEATS

## Docker Command

### Docker Cleanup Commands

1 Delete all stopped containers (including data-only containers)
```sh
$ sudo docker rm $(sudo docker ps -a -q)
```
2 Delete all 'untagged/dangling' (<none>) images
```sh
$ sudo docker rmi $(sudo docker images -q -f dangling=true)
```
3 Delete ALL images
```sh
$ sudo docker rmi $(sudo docker images -q)
```
4 Kill all running containers
```sh
$ sudo docker kill $(sudo docker ps -q)
```
### Docker Run

1 Bash
```sh
$ sudo docker run -i -t --entrypoint /bin/bash <IMAGE_ID>
$ sudo docker exec -it <CONTAINER_ID> bash
```
## Docker Compose Command

1 Build
```sh
 $ sudo docker-compose build
```
2 Start container
```sh
 $ sudo docker-compose up -d
```
3 Logs
```sh
 $ sudo docker-compose logs
```
4 Stop container
```sh
 $ sudo docker-compose stop
``` 
