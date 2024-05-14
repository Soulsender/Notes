# Creating a VM Instance
```
gcloud compute instances create gcelab2 --machine-type n1-standard-2 --zone $ZONE
```

- `gcloud compute` is used to manage compute engine resources
- `instances create` creates a new instance
- `gcelab2` is the name of the instance
- `--machine-type` flag specifies the machine type as n1-standard-2
- `--zone` specifies the zone where the VM is created
- if `--zone` is omitted, gcloud will use your zone based on default properties
- `$ZONE` in this case is a shell variable I set to a `us-east1-b`

# Firewall
EXAMPLE: 
```
gcloud compute firewall-rules create default-allow-http --direction=INGRESS --priority=1000 --network=default --action=ALLOW --rules=tcp:80 --source-ranges=0.0.0.0/0 --target-tags=http-server
```

# Kubernetes & Clusters
## Set default zone
```
gcloud config set compute/zone us-central1-a
```
## Create a cluster
```
gcloud container clusters create test-cluster
```

## Get auth credentials
```
gcloud container clusters get-credentials test-cluster
```

## Deploying a hello world app
```
kubectl create deployment hello-server --image=gcr.io/google-samples/hello-app:1.0
```
- create a kubernetes service that exposes the app
```
kubectl expose deployment hello-server --type=LoadBalancer --port 8080
```
- check if it's running
```
kubectl get service
```

## Delete the cluster
```
gcloud container clusters delete test-cluster
```