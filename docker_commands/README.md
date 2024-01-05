**Docker commands**

**Docker build .** -> builds the docker imager docker run <image_id> -> runs the id
**Docker ps** -> lists the running containers
**Docker ps -a** -> lists all the containers

**Docker run -p 8000:80 <image_id>** -> if u want to run the container in port 80, add -p exclusively to the command.

**Docker run -p 8000:30 -d <image-id>** -> if u want to run the container in detach mode.

**Docker ps 
Docker attach <container_name>** -> if u want to attach to a container. 

**Docker logs <container-name>** -> gives the logs history

**Docker logs -f <container_name>** -> gives the logs history and also attach the container

**Docker stop <container-name>** -> stops a container
**Docker start <container-name>** -> starts a container in detach mode by default.
**Docker start -a <container-name>** -> starts a container in attach mode

**Docker run -it <image-id>**  -> if you want to give an input string.

**Docker start -a -I <container-name>** -> able to start a stopped container and in attach and interactive mode(to input strings)

**Delete a container: 
	Docker rm <container_name>** -> removes the container. You have to first stop the 	container to remove/delete it. 
	**Docker rmi <image-id>** -> removes the images. 
	**Docker run -rm <image-id>** -> removes the container automatically once 			stopped. 

**Inspect:
	Docker images inspect <image-id>** -> gives the complete log about the image

**Copy file or folder to container:**
	If you want to copy a file or folder into a running contatiner:
	**Docker cp src dst**
	For eg:
	**Docker cp dummy/. <container_name>:/app/test**

**Naming and tagging containers and images:
	docker run - -name <container-name> <image-id>**

**Pushing Images to Docker hub:
	docker push <imageid>
	docker login
	docker tag <old container name> <new container name>**
 
**Pulling Imgaes from docker hub:
	docker pull <containername>**
