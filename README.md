# compsetest_docker
- docker images will show all top level images, their repository and tags, and their size.
<img width="937" alt="Screenshot 2022-10-11 110241" src="https://user-images.githubusercontent.com/63906551/195048845-5415e98b-b811-4517-ab26-3ec4a6f9f1b7.png">
 
 - Docker info displays system wide information regarding the Docker installation<img width="949" alt="Screenshot 2022-10-11 110805" src="https://user-images.githubusercontent.com/63906551/195049398-438ea03d-c04a-453c-92dc-cc1e124f77d6.png">


### Pull an image from Docker Hub
- To download a particular image, or set of images (i.e., a repository), use docker pull. If no tag is provided, Docker Engine uses the :latest tag as a default. This command pulls the debian:latest image:<img width="960" alt="Screenshot 2022-10-11 111519" src="https://user-images.githubusercontent.com/63906551/195050156-fc739c1b-68a6-4829-8a9e-b0388c22f606.png">


### Show both running and stopped containers
-The docker ps command only shows running containers by default. To see all containers, use the -a (or --all) flag:<img width="956" alt="Screenshot 2022-10-11 112054" src="https://user-images.githubusercontent.com/63906551/195051373-63115ce0-5c0d-4366-8570-1dda5c4bc3f7.png">


### Push a new image to a registry
- First save the new image by finding the container ID (using docker container ls) and then committing it to a new image name. Note that only a-z0-9-_. are allowed when naming images:
-docker tag image id dockerhubusername/imagename:mytag
To login
- docker login docker.io
- docker push dockerhubusername/imagename:mytag
<img width="939" alt="Screenshot 2022-10-11 115819" src="https://user-images.githubusercontent.com/63906551/195062117-199db02a-f989-427d-9e01-5b369e440072.png">


- remove a running container
This command removes a running container/Images.
docker rmi debian
<img width="920" alt="Screenshot 2022-10-11 121621" src="https://user-images.githubusercontent.com/63906551/195064624-8a4e5cca-a9c2-4398-a0cb-da6cd1e8ea65.png">


#### Run a command in a new container

-Usage
 docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
 <img width="920" alt="Screenshot 2022-10-11 121621" src="https://user-images.githubusercontent.com/63906551/195065252-6657c376-3228-4ee5-9577-f1b609810c1e.png">

- docker compose up -d
- docker compose run web env<img width="949" alt="Screenshot 2022-10-11 122753" src="https://user-images.githubusercontent.com/63906551/195067028-3dccde35-e8db-4337-bd14-e3ee616b937e.png">

- docker compose down --volumes
