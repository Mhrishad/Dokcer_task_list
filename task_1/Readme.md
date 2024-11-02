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

