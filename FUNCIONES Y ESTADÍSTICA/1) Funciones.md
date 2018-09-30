# Funciones y Estadística

## DESAFIO

![Screenshot](https://github.com/CarlosBrignardello/ExcelApuntes/blob/master/IMAGENES/IMAGEN%201.jpg)

## DESARROLLO

#### 1) ¿Cual es el promedio mayor?

Para poder resolver este ejercicio se requiere del uso de la función ``=PROMEDIO()`` la cual ya estaba creada automáticamente , si investigas un poco mas notaras que la formula dentro de los resultados es la siguiente ``=PROMEDIO(D7:D12)`` , Entonces lo mejor que se puede hacer es utilizar la función Max y utilizar de rango todos los promedios.

**Formula:** ``=MAX(H7:H12)``

**Resultado: 6,2**

#### 2) ¿Cuál es el promedio menor?

Lo mismo de antes solo que ahora utilizamos la función ``=MIN()``.

**Fomula:** ``=MIN(H7:H12)``

**Resultado: 3,4**
 
#### 3) ¿Cuál es la nota mayor?

Para poder obtener el resultado apropiado simplemente utilizamos como rango todas las notas de las tres pruebas.

**Formula:** ``=MAX(D7:F12)``

**Resultado: 7,0**

#### 4) ¿Cuál es la nota menor?

Lo mismo de antes soloo que ahora con la función ``MIN()``.

**Formula:** ``=MIN(D7:F12)``

**Resultado: 2,1**

#### 5) ¿Cuántas notas superiores a 4 hay en las 3 pruebas?

Para saber sobre cantidad utilizamos la función ``CONTAR.SI()``. Pues nos permite además añadir condiciones , en este caso ``>4``.

**Formula:** ``CONTAR.SI(D7:F12;">4")``

**Resultado: 12**

#### 6) ¿Cuántas notas inferiores a 4 hay en las 3 pruebas?
Lo mismo que antes solo que ahora como condición añadimos el ``<4``.

**Formula:** ``=CONTAR.SI(D7:F12;"<4")``

**Resultado: 6**

#### 7) ¿Cuántos alumnos están reprobados en la asignatura?

Para poder obtener este valor volvemos a utilizar la herramienta ``CONTAR.SI()`` y utilizamos la misma condición anterior , solo que ahora , utilizamos el promedio automatico como rango.

**Formula: ``CONTAR.SI(H7:H12;"<4")``

**Resultado : 1**


#### 8) ¿Cuántos alumnos están aprobados en la asignatura?

Repetimos el caso anterior solo que únicamente cambiamos la condición a ``>4`` para asegurarnos que sean alumnos aprobados.

**Formula: ``CONTAR.SI(H7:H12;">4")``

**Resultado: 5**

#### 9) ¿Cuál es el promedio general de los alumnos aprobados en la asignatura?

Utilizamos la función ``PROMEDIO.SI()``. Para promediar el rango seleccionado y añadir un condición , en estecaso ``>=4``.

**Formula: ``=PROMEDIO.SI(H7:H12;">=4")``

**Resultado: 4,96**


#### 10) ¿Cuál es el promedio general en la asignatura para las alumnas?

Para poder sacar este promedio dependemos una condición (en este caso el sexo de los estudiantes) para ello utlizamos ``PROMEDIO.SI()`` y añadimos el rango donde se aplicara la condición , la condición en si misma y finalmente el rango que se sumara si se cumple la condición.

**Formula: ``=PROMEDIO.SI(C7:C12;"F";H7:H12)``

**Resultado: 5,5**

#### 11) ¿Cuántos hombres hay en el listado?

En esta ejercicio debemos utilizar ``CONTAR.SI()`` pues nos piden contar un dato y ademas nos ponen una condición , en la condicion simplemente escribimos ``"M"``.

**Formula:** ``CONTAR.SI(C7:C12;"M")``

**Resultado: 4**

#### 12) ¿Cuántos hombres están reprobados?

**Formula:** ``CONTAR.SI.CONJUNTO(C7:C12;"M";H7:H12;"<4")``

**Resultado: 1**

#### 13) ¿Cuál es el promedio en la Prueba 1 de los alumnos(as) aprobados?

Hacemos uso de ``PROMEDIO.SI()`` , en rango ponemos donde evaluaremos el criterio (alumnos aprobados) y en rango_criterio pondremos el rango de toda la prueba 1.

**Formula:** ``PROMEDIO.SI(H7:H12;">=4";D7:D12)`` & ``PROMEDIO.SI.CONJUNTO(D7:D12;H7:H12;">=4")``

**Resultado: 5,3** 

#### 14) ¿Cuántos alumnos tienen nota superior a 4 en la Prueba 1 y Prueba 2?

**Formula:** ``CONTAR.SI.CONJUNTO(D7:D12;">4";E7:E12;">4")``

**Resultado: 2**

#### 15) ¿Cuántos hombres tienen nota superior a 4 en la Prueba 1 y Prueba 3?



**Formula: ``CONTAR.SI.CONJUNTO(C7:C12;"M";D7:D12;">4";F7:F12;">4")``

**Resultado: 2**

#### 16) ¿Cuál es la suma de notas en la Prueba 1 para las mujeres?




**Formula:** ``SUMAR.SI(C7:C12;"F";D7:D12)``

**Resultado: 10**

#### 17) ¿Cuál es la suma de notas en la Prueba 1 y 3 para las mujeres?



**Formula:** ``SUMAR.SI(C7:C12;"F";D7:D12) + SUMAR.SI(C7:C12;"F";F7:F12)``

**Resultado: x**

#### 18) ¿Cuántos alumnos tienen un promedio superior o igual al promedio general del curso?



**Formula:** ``CONTAR.SI(H7:H12;">=" & H13)``

#### 19) ¿Cuántos alumnos comienzan con la letra J en su nombre?
CONTAR.SI(B7:B12;"J*")

#### 20) ¿Cuál es el promedio general obtenido en la Prueba 1 y Prueba 3?
(D13+ F13)/2
PROMEDIO(D13;F13)
PROMEDIO(D7:D12;F7:F12)
