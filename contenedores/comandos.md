## Contenedor

### Check version
```
docker version
```

### Start container
```
docker container run -it ubuntu:latest bash
```

### List containers
```
docker container ls
```

### List containers -a
```
docker container ls -a
```

### Eliminar contenedor
```
docker container stop <name>
docker container rm <name>
```

### Reiniciar contenedor con politicas de reinicio
```
docker container run --name neversaydie -it --restart always alpine sh
```

### Crea un nuevo proceso dentro del contenedor
```
docker container exec <name-contenedor>
```