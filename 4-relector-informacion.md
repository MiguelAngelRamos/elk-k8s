Para recoger los logs de tus pods en k8s y enviarlos a Elaticssearch

## Instalar Filebeat

```sh
helm install filebeat elastic/filebeat --version 7.17.3
```

Filebeat detectará los logs de los pods y los enviara a Elaticssearch automáticamente.