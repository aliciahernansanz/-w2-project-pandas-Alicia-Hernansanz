# w2-project-pandas-Alicia-Hernansanz


### Comprobaciones y limpieza del Data set a nivel general


Una vez importado el csv, comprobamos el tamaño del data set. (25723, 24)

Luego el memory usage, para tener una idea de la cantidad de valores nulos por columna.



Eliminamos duplicados, para poder limpiar unas cuantas filas.
Las filas pasan de ser 25723 a 6312.

Despues pasamos a limpiar las columnas, comprobamos el % d evalores nulos en cada una de ellas.
Tan solo hay 2 que tengan más del 80% de sus valores nulos.
Estas dos (unnamed:22,unnamed:23), son eliminadas.
Las columnas pasan de ser 24 a 22.

Por último, a nivel de limpieza general del datat frame, buscamos filas con gran cantidad de nulos.
Para ello trasponemos los valores y filtramos por mas de 7 nulos por fila (un 30% apprx).
Con esto conseguimos reducir las filas de 6312 a 6295.

Siguiente paso es limpiar el nombre de las columnas.
Eliminamos los posibles espacion que esten antes o depsues de las palabras.
Y convertimos todo a minusculas.


### Comprobaciones y limpieza del Data set a nivel columna

Primero la columnas case number, para que sirva de referencia en cuanto a fechas. Ya que es la mas completa de todas las que aportan valores similares.
Sustituimos sus valores nulos por 'unknown'.
Después eliminamos todos los caracteres que esten fuera del formato yyyy/mm/dd.

type
fatal
sex
year
species

cross table para ver la relacion entre fatal accidents segun el tipo de especie


