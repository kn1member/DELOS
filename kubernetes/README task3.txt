Task 3:
mongoDB basics

FINISHED: 
- Deploy mongoDB in Kubernetes:
	- Go to kubernete directory, open terminal/cmd as administrator, type this command:
kubectl apppy -f mongo-secret.yaml (apply the secret username and password first)
kubectl apppy -f mongo.yaml (create mongo deployement & service)
kubectl apppy -f mongo-configmap.yaml (define configuration variables for deploying mongo-express)
kubectl apppy -f mongo-express.yaml (define configuration variables for deploying mongo-express)
minikube service mongo-express-service --url sa-frontend-lb (run mongo express in http://ip-address:30000)

NOT FINISHED:
-Set a collection in mongoDB (the format of the collection is up to you)
-Set a pod and container that inserts a few records into the mongoDB collection; the code inside the container must be in python and do not use shell commands inside yaml files

