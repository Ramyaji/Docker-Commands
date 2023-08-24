https://docs.docker.com/engine/reference/commandline/docker/
https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands
reference above links for commands
# Docker-Commands
Docker-commands
Docker Commands:

Managing Images and Containers:
docker pull <image_name>: Pull an image from a registry.
docker build -t <image_name> <path_to_Dockerfile>: Build a Docker image from a Dockerfile.
docker run -d --name <container_name> <image_name>: Run a container from an image.
docker ps: List running containers.
docker ps -a: List all containers (including stopped ones).
docker stop <container_name>: Stop a running container.
docker rm <container_name>: Remove a container.
docker rmi <image_name>: Remove an image.
docker exec -it <container_name> <command>: Run a command inside a running container interactively.
Managing Volumes and Networking:
docker volume create <volume_name>: Create a Docker volume.
docker volume ls: List Docker volumes.
docker network create <network_name>: Create a Docker network.
docker network ls: List Docker networks.
Docker Compose (for managing multi-container applications):
docker-compose up: Start services defined in a Docker Compose file.
docker-compose down: Stop and remove containers, networks, and volumes defined in a Docker Compose file.

Kubernetes Commands:

Cluster Management:
kubectl cluster-info: Display information about the cluster.
kubectl get nodes: List all nodes in the cluster.
kubectl get pods: List all pods in the cluster.
kubectl get services: List all services in the cluster.
Deployment and Scaling:
kubectl create deployment <deployment_name> --image=<image_name>: Create a deployment.
kubectl scale deployment <deployment_name> --replicas=<replica_count>: Scale a deployment.
kubectl rollout status deployment <deployment_name>: Check the rollout status of a deployment.
Managing Pods and Containers:
kubectl get pods: List pods.
kubectl describe pod <pod_name>: Get detailed information about a pod.
kubectl logs <pod_name>: Display the logs of a pod.
kubectl exec -it <pod_name> -- <command>: Execute a command inside a pod interactively.
Services and Networking:
kubectl expose deployment <deployment_name> --type=<service_type> --port=<port>: Expose a deployment as a service.
kubectl get services: List services.
kubectl describe service <service_name>: Get detailed information about a service.
Configuration and Secrets:
kubectl create configmap <configmap_name> --from-file=<file_path>: Create a ConfigMap from a file.
kubectl create secret generic <secret_name> --from-literal=<key>=<value>: Create a secret.
kubectl get configmaps: List ConfigMaps.
kubectl get secrets: List secrets.
