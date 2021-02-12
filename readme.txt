Flask app deployed on Kubernetes locally

Commands to run Kubernetes:

 cd hello-python/app
 sudo docker build -t hello-python .
 sudo docker run --name myapp2 -p 5000:5000 hello-python:latest
 sudo usermod -aG docker $USER && newgrp docker
 minikube start
 kubectl apply -f deployment.yaml
 kubectl get pods
 minikube service list