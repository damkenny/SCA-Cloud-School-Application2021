# SCA-Cloud-School-Application


SCA-Cloud-School-Application-
Tools used: Docker,Node:Alpine, VisualStudioCode, Git, Github.

Step 1. Creating a Directory for the Webpage

A repository was created and cloned into visualstudio code which create a directory on my PC which include a simple app.js to display "Welcome to SCA Cloud School Application" and a docker file with the following command" FROM node:alpine COPY . /app WORKDIR /app CMD node app.js " which was copying the content (images) of the directory into the container.

The docker desktop was downloaded on my Virtual Machine, was running locally and online on the docker hub becuase it has to be running before the docker file can be created.

Step 2. Creating the first image

The below command was use to create an image which was runned and tested in a container.

   cmd -- docker build . -t kehindeafusat/mujy:V1 . This created the first image, then I created a tag muji:V1 to create on the image on local repository which requires me creating a tag TARGET_IMAGE that refers to SOURCE_IMAGE

C:\Users\kenny\sca3\SCA-Cloud-School-Application\docker>docker tag mujy:V1 kehindeafusat/mujy then I pushed the first image to docker using docker push kehindeafusat/mujy:V1 ans ran thr container.

Output:"Welcome to SCA Cloud School Application".

Step 3. Testing the image and running the docker container.

The command -- docker container ls-- was used to check if there are any container running and docker container stop  (to stop the container running on a port) using the port 80 or port 8080 to display the webpage with the text "Welcome to SCA Cloud School Application".

The command used to run the container was -- docker container run kehindeafusat/mujy:V1. 

I created the second image by building another image docker build -t mujy:V2 . then ran the container, created a tag muji:V2 to create on the image on local repository which requires me creating a tag TARGET_IMAGE that refers to SOURCE_IMAGE. 


Input: docker container run mujy:V2

Output: Welcome to SCA Cloud School Application this is my first assessment


Step 4. Pushing the final images to the docker container.

In the dockerhub, a repository called kehindeafusat/mujy was created to allow the pushing of images from the container to docker using the command -- docker push kehindeafusat/mujy

link to my dockerhub: https://hub.docker.com/repository/docker/kehindeafusat/mujy
