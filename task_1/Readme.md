nginx webserver 001
--------------------------
make a index.html file with html code
write a dockerfile
take a base image of nginx
do not use the default index.html page of nginx
use the index.html file u generated
we want to browse the nginx webserver on port localhost:9090
make a docker compose file

Output:

should be able to browse the container on localhost:9090
should be able to see the custom index.html page when browsed the nginx webserver




#Build the Docker image:
    docker build -t task_1-nginx .
#Run the Docker container and map port 9090
   docker run -d -p 9090:80 --name my-nginx task_1-nginx
#With volume run
    docker run -d -p 9090:80 --name my-nginx -v "$(pwd)/index.html:/usr/share/nginx/html/index.html" task_1-nginx
#To stop and remove the container
    docker stop my-nginx
#run again
    docker rm my-nginx

