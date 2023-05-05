# ¿Que es una fork bomb?

Una fork bomb es un tipo de ataque de denegación de servicio (DoS) que utiliza un programa malicioso para agotar los recursos del sistema mediante la creación excesiva de procesos hijos (forks) que consumen la memoria y la capacidad de procesamiento del sistema.

Una fork bomb funciona mediante la creación constante de procesos hijos que a su vez crean más procesos hijos, y así sucesivamente, hasta que se agota la capacidad del sistema y se vuelve inutilizable. Este tipo de ataque puede ser extremadamente dañino y puede requerir la reinicialización del sistema para recuperarse por completo.

Es importante tener en cuenta que las fork bombs no son necesariamente maliciosas por naturaleza, y pueden ser creadas y utilizadas por programadores con fines legítimos en determinados casos. Sin embargo, cuando se utilizan con fines maliciosos, pueden causar daños importantes a los sistemas informáticos.

## Paso a paso de que hace la funcion:

Primero declaramos una funcion llamado ":" con el argumento nada, abrimos el codigo para declarar esta funcion, hacemos : para llamar a la funcion, hacemos un pay para que la salida de esa funcion se la pase a otra funcion, en este caso tambien es : y le pasamos un & para que este proceso se ponga en backgraund terminamos de declarar esta funcion y la llamamos.

Es una recurcion de una funcion para infinitos llamados a si mismo para infinitamente crear procesos.

```bash
#! bin/bash

:(){ :|:& };:
```
Es la misma sentencia que la anterior pero codificada en base64

```bash
echo “OigpeyA6fDomIH07Og==” | base64 -d
```
