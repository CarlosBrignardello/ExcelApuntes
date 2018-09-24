# Apuntes y Resolución de ejercicios en Excel

Este repositorio forma parte de mis apuntes personales sobre ofimática , respectivamente acerca del software Excel. Todos los ejemplos y referencias usadas son gracias al material universitario obtenido de la Universidad Técnica Federico Santa Maria , todo esto es básicamente un resumen muy grande con un especial analisis en la resolución de los ejercicios , si necesitas repasar o aprender Excel esto puede serte de muchísima utilidad.

## Introducción

## Resumen y Apuntes

### Funciones


#### Operadores aritméticos


Estas fórmulas combinan números, referencias de celda, funciones y operadores aritméticos. 


| Nombre        | Operador | Ejemplo | Resultado |
|---------------|----------|---------|-----------|
| Suma          | +        | =10+5   | 15        |
| Resta         | -        | =10-5   | 5         |
| Negación      | -        | =-10    | -10       |
| Multiplicación| *        | =10 * 5 | 50        |
| División      | /        | =10/5   | 2         |
| Porcentaje    | %        | =10%    | 0.1       |
| Exponente     | ^        | 10^5    | 100000    |


#### Operadores de comparación


Permiten comparar números o cadenas de texto. Los valores positivos dan como resultado el valor VERDADERO. Lo mismo pasa en caso contrario obteniendo el resultado FALSO.

| Nombre            | Operador | Ejemplo | Resultado |
|-------------------|----------|---------|-----------|
| Mayor que         | >        | =15>5   | VERDADERO |
| Menor que         | <        | =10<5   | FALSO     | 
| Igual a           | =        | =10=5   | FALSO     |
| Mayor que         | >        | =15>5   | VERDADERO |
| Menor que         | <        | =10<5   | FALSO     |
| Mayor o igual que | >=       | =10>=5  | VERDADERO |
| Menor o igual que | <=       | =10<=5  | FALSO     |
| Diferente de <>   | <>       | =10<>5  | VERDADERO |


#### Operadores de texto


Los operadores de texto permiten manipular el texto.

| Nombre        | Operador | Ejemplo                    | Resultado          |
|---------------|----------|----------------------------|--------------------|
| Concatenación | &        | =”Carlos” & “Brignardello” | CarlosBrignardello |


#### Operadores de referencia


Los operadores de referencia sirven para combinar referencias de celda para crear una única referencia.

| Nombre       | Operador  | Resultado                                                       |
|--------------|-----------|-----------------------------------------------------------------|
| Rango        | :         | Produce un rango entre dos referencias de celda (A1:D5)         |
| Unión        | , o ;     | Produce un rango que es la unión de dos rangos (A1:D5,F1,H5)    |
| Intersección | (espacio) | Produce un rango con celdas comunes de dos rangos (A1:D5 B3:F8) |


#### Referencias absolutas


Si queremos mantener fija una celda de modo que al copiarla en otra celda no cambie su referencia lo único que tenemos que hacer es incluir el símbolo ``$``

Referencia Relativa : ``A7``

Referencia Absoluta : ``$A$7``

Nota : También puedes pulsar F4 al momento de escribir las referencias para que se haga automático.


#### Referencias a celdas en otra hoja


Aveces podemos llegar a necesitar utilizar valores que se encuentran en otras hojas , para ello podemos utilizar la siguiente función : ``=’Hoja2’!C5``


### Funciones Aritmeticas


#### SUMA()


| Función                 | Descripción                                       | Resultado |
|-------------------------|---------------------------------------------------|-----------|
| =SUMA(3;2)              | Suma 3 y 2                                        | 5         |
| =SUMA(“5”;15;VERDADERO) | Suma 15 y 1                                       | 16        |
| =SUMA(A2:A4)            | Suma los  valores contenidos entre esas dos celdas| X         |


#### SUMAR.SI()


Sumar.Si tiene un rango , un criterio y un rango_suma

| Nombre    |                                                        Descripción                                                   |
|-----------|----------------------------------------------------------------------------------------------------------------------|
|Rango      | Son los valores que se desean evaluar , pueden ser (como dicen el nombre) rangos                                     |
|Criterio   | El criterio es una condición que debe cumplir el dato que este contenido en el rango                                 |
|Rango_Suma | El rango_suma son las celdas que se van a sumar en caso de que el valor contenido en el rango cumple con el criterio |

Mas adelante se detallara esta función.


#### SUMAR.SI.CONJUNTO()


Sumar.Si.Conjunto contiene rango_suma , rango_criterios1 criterios1 y asi infinitamente. Sirve muchísimo si se necesita realizar lo mismo que un Sumar.Si pero varias veces y con valores y condiciones distintas.

| Nombre          |                                          Descripción                                         |
|-----------------|----------------------------------------------------------------------------------------------|
|Rango_suma Es    |el rango de los valores que se van a sumar si se cumplen el resto de condiciones asociadas    |
|Rango_criterios1 |Es el primer rango en el que se evaluaran las condiciones                                     |
|Criterios1       |Son las condiciones que se requieren para hacer las pertinentes sumas en los rangos anteriores|


*Estos dos últimos procesos se pueden repetir infinitamente.


---
Con ❤️ por [CarlosBrignardello](https://github.com/carlosbrignardello) 😊
