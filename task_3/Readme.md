#Build docker file for react app
   docker build -t my-react-app:latest .
#run the docker file
    docker run -d -p 3000:3000 --name running-react-app my-react-app:latest
#stop 
    docker stop running-react-app
#remove container
    docker rm running-react-app

Docker image name : mhrishad/reactapp:latest  & mhrishad/reactapp:node-14 

Docker Compose up -d detached mode 

docker-compose up -d
