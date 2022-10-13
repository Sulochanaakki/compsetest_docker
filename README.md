# compsetest_docker
 
 - To pull docker image from docker hub
 - <img width="912" alt="Screenshot 2022-10-13 093134" src="https://user-images.githubusercontent.com/63906551/195531465-55723fc2-b553-4b9e-be5a-d189a838758a.png">

- To run image
- docker run -d -p 80:80 docker/getting-started
- d - run the container in detached mode (in the background)
- p 80:80 - map port 80 of the host to port 80 in the container
- 
 <img width="905" alt="Screenshot 2022-10-13 094114" src="https://user-images.githubusercontent.com/63906551/195533419-ab445acf-9af8-4edc-a900-3ec0a9bc2994.png">

-To check the Docker image status
docker ps
 <img width="881" alt="Screenshot 2022-10-13 094335" src="https://user-images.githubusercontent.com/63906551/195533835-cef84018-a066-40aa-ae1f-09f7106449c7.png">

- To stop docker image
- docker stop containerid
- <img width="899" alt="Screenshot 2022-10-13 094837" src="https://user-images.githubusercontent.com/63906551/195535142-031fd798-1ee0-4713-8df6-23f1caafcc43.png">

-To stop docker image
docker stop containerid
<img width="898" alt="Screenshot 2022-10-13 095331" src="https://user-images.githubusercontent.com/63906551/195536057-7d15dd65-f879-4346-9d7c-43359bc51174.png">

-To remove docker image
docker rm image Id
_ to remove forcefully
dcoker rm -f image Id
<img width="878" alt="Screenshot 2022-10-13 095847" src="https://user-images.githubusercontent.com/63906551/195537184-9a8c0426-038a-452a-8748-13d34efaaad8.png">







 
 
 
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
