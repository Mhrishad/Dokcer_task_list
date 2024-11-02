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




React app
--------------------------------------------------------------------
lets go to the react documentation
figure out the prerequisite software packages required to run react
download them
then figure out how to generate a react demo application
run it locally
then make a docker file
figure out what to write in docker file to run the react application
now push the same image to your dockerhub with 2 tags
reactapp:latest
reactapp:base_image_you_used
now make a docker compose file
refer docker compose to use that image
expose ports
run