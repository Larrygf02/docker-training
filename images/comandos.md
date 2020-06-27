## Obtener todas las imagenes

```
docker images ls
```
## Tirar de una imagen (extracción)

```
docker image pull ubuntu:latest
```

## Etiquetado de imagenes
```
docker image pull <repository>:<tag>
```
* Si no se especifica el tag, pone por defecto el ultimo
* Una imagen puede tener tantas etiquetas como desee

## Descargar todas las versiones de una imagen
```
docker image pull -a <repository>
```
## Filtrar imagenes
```
docker image ls --filter dangling=true
docker image ls --filter before=<id-image>
```

## Filtrar images con tag latest
```
docker image ls --filter=reference="*:latest"
```

## Format output images
```
docker image ls --format "{{.Size}}"
```

## Buscando Docker Hub
```
docker search <repository>
docker search <repository> --filter "is-official=true"
```