## Comandos para ver el uso de recursos del cluster de Minikube
### Windows
```sh
kubectl describe node | findstr /I /C:"Capacity" /C:"cpu:" /C:"memory:"
```
### Linux
```sh
kubectl describe node | grep -A3 "Capacity"
```

Si tienes pocos recursos asignados el cluster de minikube siempre puedes asignarle mas recursos en el arranque.

```sh
minikube start --memory=8192 --cpus=4
```

En este ejemplo arrancamos con 8gb en ram y cpus 4 