## Paso 1

Verifica que minikube y kubectl estan disponibles

```sh
minikube status
kubectl get nodes
```
## Paso 2

Habilita el dashboard 

```sh
minikube addons enable dashboard
```

Instala Helm (Helm es el gestor de paquetes para Kubernetes)

```sh
choco install kubernetes-helm
```

## Agregar el repositorio de Elastic

```sh
helm repo add elastic https://helm.elastic.co
```
```sh
helm repo update
```