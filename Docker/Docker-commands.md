Build Docker Image.
docker build -t jags-shopping:v1 .

List the images
docker images

Run Docker container
docker run -d --name jags-app -p 8080:80 jags-shopping:v1

List running containers
docker ps

Tag Image
docker tag jags-shopping:v1 674113923535.dkr.ecr.us-east-2.amazonaws.com/jags-shopping:v1

Push docker image to ECR
docker push 674113923535.dkr.ecr.us-east-2.amazonaws.com/jags-shopping:v1

