# Sample container app

Sample dotnet 6.0 minimal api to run in docker and kubernetes. This app is a regular "Hello World!" app. I generally use this while demoing concepts using containers and kubernetes. I have been trying to make the container size as small as possible. It is currently 43.23 MB.

## To Run

This app is too simple to be used on its own. It makes sense to use it in a container as a sample app.

### Docker

docker run --rm -p 8000:8080 -e TARGET=Universe pradeepl/helloworld:latest  
curl http://0.0.0.0:8000

### Kubernetes

Create a deployment and use the image