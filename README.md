# kubernetes-orientdb-distributed
This is temporary repository to explain the OrientDB scaling and replication in kubernetes

## Prerequisite
- Windows 10
- Docker Desktop CE
- Enable Kubernetes in Docker Desktop CE

## Build docker Image
OrientDB with hazelcast configuration
``
docker build -t orientdb-dist ./distributed
``
## Helm
``
helm init
``

## Install Ingress Controller
``
helm install stable/nginx-ingress --version 1.1.5 --name lb
``

## Apply Ingress rule
``
kubectl apply -f ./ingress
``
## OrientDB 
``
kubectl apply -f ./
``

Docker drive share issue help link:
https://stackoverflow.com/a/46854772/1629967




