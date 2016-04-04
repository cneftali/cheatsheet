# My Docker FAQ / TIPS

## Docker Command

### Docker Cleanup Commands

  1. Delete all stopped containers (including data-only containers)
      
      $ sudo docker rm $(sudo docker ps -a -q)

  2. Delete all 'untagged/dangling' (<none>) images

      $ sudo docker rmi $(sudo docker images -q -f dangling=true)

  3. Delete ALL images

      $ sudo docker rmi $(sudo docker images -q)

  4. Kill all running containers

      $ docker kill $(sudo docker ps -q)


## Docker Compose Command

  1. Build

     $ sudo docker-compose build

  2. Start container

     $ sudo docker-compose up -d

  3. Logs

     $ sudo docker-compose logs

  4. Stop container

     $ sudo docker-compose stop 