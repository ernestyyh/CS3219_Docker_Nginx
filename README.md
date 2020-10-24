# CS3219 Docker & Nginx
Task: To deploy a simple web server using Nginx running in a Docker container.

## Running Docker image locally

### By pulling Docker image from Docker Hub
1. Pull image from Docker Hub: <br>
````sh
docker pull ernestyyh/nginx_server
````
2. Run the container: <br>
````sh
docker run -p 80:80 --rm -d --name nginx_rp ernestyyh/nginx_server
````

### By cloning repository to a local directory
1. Clone the repository: <br>
````sh
git clone https://github.com/ernestyyh/CS3219_Docker_Nginx
````
2. Build the Docker image: <br>
````sh
docker build -t server .
````
3. Run the container: <br>
````sh
docker run -p 80:80 --rm -d --name nginx_server server
````
