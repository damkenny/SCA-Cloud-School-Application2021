# SCA-Cloud-School-Application


SCA-Cloud-School-Application-
Tools used: Docker,Node:Alpine, VisualStudioCode, Git, Github.

Step 1. Creating a Directory for the Webpage

A repository was created and cloned into visualstudio code which create a directory on my PC which include the landing page index.html file, an html file to display "Welcome to SCA Cloud School Application" and a docker file with the following command" FROM node:alpine COPY . /app WORKDIR /app CMD node app.js " which was copying the content (images) of the directory into the container.

The docker desktop was downloaded on my Virtual Machine, was running locally and online on the docker hub becuase it has to be running before the docker file can be created.

Step 2. Creating the image

The below command was use to create an image which was runned and tested in a container. cmd -- docker build . -t kehindeafusat/magik:V1. cmd -- docker images -- was used to check for the images created.

Step 3. Testing the image and running the docker container.

The command -- docker container ls-- was used to check if there are any container running and docker container stop  (to stop the container running on a port) using the port 80 or port 8080 to display the webpage with the text "Welcome to SCA Cloud School Application".

The command used to run the container was -- docker container run -p 80:80 kehindeafusat/mabby:latest. (The first 80 is the port docker is running on the second 80 is the local port to run a container on port 80 which is repository name is mabby and tag is latest)

Output: docker container run -p 8080:80 kehindeafusat/mabby:latest Welcome to Cloud school application, this is my first assessment


Step 4. Pushing the images to the docker container.

In the dockerhub, a repository called kehindeafusat/mabby was created to allow the pushing of images from the container to docker using the command -- docker push kehindeafusat/mabby:latest

link to my dockerhub: https://hub.docker.com/repository/docker/kehindeafusat/mabby
