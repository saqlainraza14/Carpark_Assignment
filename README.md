# Deploying a Static HTML Site with Docker


 Create a Directory for the Website<br />
 
 Create a file called Dockerfile<br />
 	 FROM nginx:alpine<br />
 	 COPY . /usr/share/nginx/html<br />

Build the Docker Image<br />
  	docker build -t html-server-image:v1<br />

Command to check all available image<br />
  	docker images<br />
Run the Docker Container<br />
  	docker run -d -p 8080:80 html-server-image:v1<br />
Test the Port<br />
  	http://localhost:8080/<br />
