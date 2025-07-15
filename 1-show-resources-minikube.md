## Comandos para ver el uso de recursos del cluster de Minikube
### Windows
```sh
kubectl describe node | findstr /I /C:"Capacity" /C:"cpu:" /C:"memory:"
```
### Linux
```sh
kubectl describe node | grep -A3 "Capacity"
```