```
- minikube start
- eval $(minikube docker-env)  // to point the docker images inside of minikube, only then will the build be read by kubernetes.
- minikube docker-env
- docker build <file> -t <name>:<tag>
- kubectl create deployment <deployment> --image=<image name>:<tag>
- kubectl get pods
- kubectl get deployments

- kubectl create service loadbalancer <deployment name> --tcp=3000:3000
    or
- kubectl expose deployment <service name> --type="LoadBalancer" --post=<execution port>    // expose the service as "Load Balancer" to interact with the pod ( our container )

- kubectl get services
- minikube service <service> --url     // to get the url of the service
- minikube dashboard
- kubectl proxy // to use browser to work with kube. Will return a url.
```
