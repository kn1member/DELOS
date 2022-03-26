Task 1: 
Kubernetes basics
FINISHED:
-Create 2 pods that communicate by means of a service;
	- install minikube (using for creating virtual machine)
	- install kubectl (using for creating pods, deployments, services,...)
	- minikube start --driver=hyperv (can user other virtual machine: virtualbox, hyperkit,..)
-Sample code to demonstrate Dockerfile function

NOT FINSISHED:

-Pod 1 sends ‘hello word’ to pod 2 which reads it and prints it out; pod 2 keeps sending ‘I got it, roger’ to pod 1 which prints out this message
You must create a deployment and service yaml files; the two pods must be deployed by using ‘kubectl apply’ and the service must also be deployed in the same way
Each pod reads from a configmap file the average time between sending two messages to the other file (thus the configmap has two values); Use uniform distribution in the range [a/2, 3a/2] where a is the average read from the configmap
The server-client portion of the code must be written in Python
The configmap file must be set as a configmap that is mounted to the pod

-You must create a Dockerfile for the two containers behind the two pods and do not use shell commands inside yaml files.

