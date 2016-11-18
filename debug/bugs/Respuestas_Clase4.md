1.- Archivo "add_array_static"
Hay un error en la utilización de los índices. 
El primer "for" debería correr hasta i<n.

2.- Archivo "add_array_segfault"
Los punteros están mal definidos. Habría que utilizar "malloc" para reservar memoria en forma dinámica.

Al agregar los flags se puede tener una idea de dónde suceden los problemas. Con el flag -g se ve que el error está en "main", con el flag -wall aparece la línea en donde sucede el problema.

3.- Archivo "add_array_dynamic"
Los punteros están bien definidos. No hay errores.

4.- Archivo "add_array_nobugs"
Las variables están definidas como vectores. No hay errores.


Segmentation fault
Al ejecutar ulimit -s unlimited, se aumenta temporariamente la asignación de memoria, pero en esa terminal y en ese momento. Entonces, no se resuelve realmente el problema. Una forma de subsanarlo sería asignando memoria en forma dinámica







 
