# ptmalloc2

Implementación de la librería [ptmalloc2](http://www.malloc.de/en/)

## Introducción
Implementación de la librería [ptmalloc2](http://www.malloc.de/en/) para el estudio del la gestión de memoria dinámica dentro de los ejecutables ELF

### Implementación

Compilar ptmalloc2
```
make linux-pthread
```

Integración de la librería
```
gcc example.c libmalloc.a -pthread -o example
```