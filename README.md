# Kubernetes Sidecar Pattern Demo

This project demonstrates the Kubernetes Sidecar Pattern using a multi-container Pod. The main container writes data to a shared `emptyDir` volume, while the sidecar container continuously reads and displays the data from the same shared storage.

## Features

* Multi-container Pod deployment
* Shared storage using `emptyDir`
* Sidecar container communication
* Pod inspection using `kubectl describe`
* Log monitoring using `kubectl logs`
* Kubernetes YAML manifest configuration

## Technologies Used

* Kubernetes
* YAML
* BusyBox
* emptyDir Volume
* kubectl

## Learning Outcomes

* Understanding the Sidecar Pattern
* Working with shared volumes
* Managing multi-container Pods
* Monitoring container logs
* Troubleshooting Kubernetes workloads

## Commands Used

kubectl apply -f side-car.yaml

kubectl get pods -o wide

kubectl describe pod sidecar-practice

kubectl logs sidecar-practice -c side-car-container
