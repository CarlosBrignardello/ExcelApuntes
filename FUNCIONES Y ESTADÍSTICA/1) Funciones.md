# Funciones y Estadística

## DESAFIO

![Screenshot](https://github.com/CarlosBrignardello/ExcelApuntes/blob/master/IMAGENES/IMAGEN%201.jpg)

## DESARROLLO

#### 1) ¿Cual es el promedio mayor?

Respuesta : Para poder resolver este ejercicio se requiere del uso de la función =PROMEDIO() la cual ya estaba creada automáticamente , si investigas un poco mas notaras que la formula dentro de los resultados es la siguiente =PROMEDIO(D7:D12) , Entonces lo mejor que se puede hacer es utilizar la función Max y utilizar de rango todos los promedios.
=MAX(H7:H12)
Resultado : 6,2

#### 2) ¿Cuál es el promedio menor?

Respuesta : Lo mismo de antes solo que ahora utilizamos la función =MIN()
=MIN(H7:H12)
Resultado : 3,4
 
#### 3) ¿Cuál es la nota mayor?

Respuesta : Para poder obtener el resultado apropiado simplemente utilizamos como rango todas las notas de las tres pruebas.
=MAX(D7:F12)

Resultado : 7,0

#### 4) ¿Cuál es la nota menor?

Respuesta : Lo mismo de antes soloo que ahora con la función MIN()
= MIN(D7:F12)
Resultado 2,1

#### 5) ¿Cuántas notas superiores a 4 hay en las 3 pruebas?

Para saber sobre cantidad utilizamos la función CONTAR.SI()
Pues nos permite además añadir condiciones , en este caso >4

CONTAR.SI(D7:F12;">4")

Resultado: 12 

#### 6) ¿Cuántas notas inferiores a 4 hay en las 3 pruebas?
Respuesta: Lo mismo que antes solo que ahora como condición añadimos el <4
=CONTAR.SI(D7:F12;"<4")

Resultado: 6

#### 7) ¿Cuántos alumnos están reprobados en la asignatura?

Respuesta: Para poder obtener este valor volvemos a utilizar la herramienta CONTAR.SI() y utilizamos la misma conicion anterior , solo que ahora , utilizamos el promedio automatico como rango.
CONTAR.SI(H7:H12;"<4")

Resultado:1


#### 8) ¿Cuántos alumnos están aprobados en la asignatura?

Respuesta: Repetimos el caso anterior solo que únicamente cambiamos la condición a >4 para asegurarnos que sean alumnos aprobados.
CONTAR.SI(H7:H12;">4")

Resultado:5

#### 9) ¿Cuál es el promedio general de los alumnos aprobados en la asignatura?

Respuesta: utilizamos la función PROMEDIO.SI()
para promediar el rango seleccionado y añadir un condición , en estecaso >=4
=PROMEDIO.SI(H7:H12;">=4")

Resultado:4,96


#### 10) ¿Cuál es el promedio general en la asignatura para las alumnas?

Respuesta:
Para poder sacar este promedio dependemos una condición (en este caso el sexo de los estudiantes) para ello utlizamos PROMEDIO.SI() y añadimos el rango donde se aplicara la condición , la condición en si misma y finalmente el rango que se sumara si se cumple la condición.
=PROMEDIO.SI(C7:C12;"F";H7:H12)
Resultado:5,5

#### 11) ¿Cuántos hombres hay en el listado?
CONTAR.SI(C7:C12;"M")

#### 12) ¿Cuántos hombres están reprobados?
CONTAR.SI.CONJUNTO(C7:C12;"M";H7:H12;"<4")

#### 13) ¿Cuál es el promedio en la Prueba 1 de los alumnos(as) aprobados?
PROMEDIO.SI(H7:H12;">=4";D7:D12)
PROMEDIO.SI.CONJUNTO(D7:D12;H7:H12;">=4")

#### 14) ¿Cuántos alumnos tienen nota superior a 4 en la Prueba 1 y Prueba 2?
CONTAR.SI.CONJUNTO(D7:D12;">4";E7:E12;">4")

#### 15) ¿Cuántos hombres tienen nota superior a 4 en la Prueba 1 y Prueba 3?
CONTAR.SI.CONJUNTO(C7:C12;"M";D7:D12;">4";F7:F12;">4")

#### 16) ¿Cuál es la suma de notas en la Prueba 1 para las mujeres?
SUMAR.SI(C7:C12;"F";D7:D12)

#### 17) ¿Cuál es la suma de notas en la Prueba 1 y 3 para las mujeres?
SUMAR.SI(C7:C12;"F";D7:D12) + SUMAR.SI(C7:C12;"F";F7:F12)

#### 18) ¿Cuántos alumnos tienen un promedio superior o igual al promedio general del curso?
CONTAR.SI(H7:H12;">=" & H13)

#### 19) ¿Cuántos alumnos comienzan con la letra J en su nombre?
CONTAR.SI(B7:B12;"J*")

#### 20) ¿Cuál es el promedio general obtenido en la Prueba 1 y Prueba 3?
(D13+ F13)/2
PROMEDIO(D13;F13)
PROMEDIO(D7:D12;F7:F12)

#### 21) 
