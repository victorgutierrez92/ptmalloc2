# ptmalloc2

Implementación de la librería [ptmalloc2](http://www.malloc.de/en/)

## Introducción
Ejemplo de implementación de la librería [ptmalloc2](http://www.malloc.de/en/) para el estudio del la gestión de memoria dinámica dentro de los ejecutables ELF

### Implementación

1. Compilar ptmalloc2
```
make linux-pthread
```

2. Integración de la librería
```
gcc example.c libmalloc.a -pthread -o example
```

### Demostración
```
victor@ubuntu:~/Desktop$ ./ejemplo 
[DEBUG] Llamada malloc(), return: 0x08050008 (bytes=512)
[DEBUG] Llamada malloc(), return: 0x08050210 (bytes=512)
[DEBUG] Llamada unlink(), línea 4260, archivo malloc.c
```