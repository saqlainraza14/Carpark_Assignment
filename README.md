# Deploying a Static HTML Site with Docker


 Create a Directory for the Website
 
 Create a file called Dockerfile
 	 FROM nginx:alpine
 	 COPY . /usr/share/nginx/html

Build the Docker Image
  	docker build -t html-server-image:v1

Command to check all available image
  	docker images
Run the Docker Container
  	docker run -d -p 8080:80 html-server-image:v1
Test the Port
  	http://localhost:8080/
