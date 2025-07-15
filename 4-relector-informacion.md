## Logs
Para recoger los logs de tus pods en k8s y enviarlos a Elaticssearch

## Instalar Filebeat

```sh
helm install filebeat elastic/filebeat --version 7.17.3
```

Filebeat detectará los logs de los pods y los enviara a Elaticssearch automáticamente.

Menu de la izquierda, debemos seleccionar "Stack Management" -> Index Patterns

El nombre del patron es 
```
filebeat-*
```

## Ver los logs en tiempo real 
Menu de la izquierda, "Analytis" -> Discover

## Paneles 
Menu de la izquierda, "Dashboard"

## Metricas para CPU, RAM, I/O de disco, Tráfico de Red

Vamos a utilizar Metricbeat en K8s

```sh
helm install metricbeat elastic/metricbeat --version 7.17.3
```