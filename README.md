### Short list of Docker commands:

List Images: ``sudo docker images``
Example:
```
REPOSITORY      TAG                       IMAGE ID       CREATED          SIZE
payload_image   latest                    fa148686b0d3   36 minutes ago   707MB
nvidia/cuda     11.4.0-base-ubuntu18.04   fa91fba70f7f   5 weeks ago      114MB
```

Remove an Image: ``docker rmi [image_name OR image_id]`` \
Example: ``docker rmi fa14`` ``docker rmi fa14 --force``

Remove all images with prune: ``sudo docker image prune -a``

List Containers:``sudo docker ps``

List All Containers (including stopped):``sudo docker ps -a``

Remove a Container: ``sudo docker rm [container_name OR container_id]``

Stop a Container: ``sudo docker stop [container_name OR container_id]``

Start a Container: ``sudo docker start [container_name OR container_id]``

Restart a Container: ``sudo docker restart [container_name OR container_id]``

Execute a Command in a Running Container: ``docker exec -it [container_name] [command]``

Run a Container: ``sudo docker run -it [image_name] [command]``

Pull an Image from a Registry: ``sudo docker pull [image_name]``

Push an Image to a Registry: ``sudo docker push [image_name]``

Build an Image from a Dockerfile: ``sudo docker build -t [image_name] [path_to_dockerfile]``

Tag an Image: ``sudo docker tag [image_name] [new_image_name]``

**Note:** [image_name] and [container_name] should be replaced with the actual names of the image and container respectively.
