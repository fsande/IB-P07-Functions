# Práctica 07. Funciones

### Objetivos
Los objetivos de esta práctica son que el alumnado:
* Desarrolle programas sencillos en C++ que utilicen funciones y todos los tipos de sentencias estudiadas

### Rúbrica de evaluacion de esta práctica
Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva)
que se tendrán en cuenta a la hora de evaluar esta práctica:
* El alumnado ha de acreditar conocer los conceptos expuestos en el material de referencia de esta práctica.
* El alumnado ha de acreditar que ha realizado todos los ejercicios propuestos, así como ser capaz de desarrollar otros similares.
* Ha de acreditar que es capaz de escribir un fichero Makefile para automatizar el proceso de compilación de sus programas.
* El código que escriba ha de estar escrito de acuerdo a los estándares definidos en la Guía de Estilo de Google para C++.
* Todos los identificadores que utilice en su programa (constantes, variables, etc.) deberán ser
  siempre significativos. No utilice nunca identificadores de una única letra, tal vez con la excepción de las
  variables que utilice para iterar en un bucle.
* Antes de su ejecución, todos los programas que desarrolle, deben imprimir en pantalla un
  mensaje indicando la finalidad del programa así como la información que precisará del usuario para su correcta ejecución.

### Trabajo previo
Estudie en el tutorial "Fundamentos de Informática" todo el material correspondiente al capítulo
[Funciones](http://www.minidosis.org/#/temas/Cpp.Funciones)
Realice todos los ejercicios propuestos en ese capítulo.

### Ejercicios 
1. Escriba un programa `primes.cc` que solicite al usuario un número e imprima en pantalla todos los
números primos menores que el introducido por el usuario
```
Introduzca un número: 100
2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97
```
El programa ha de contener una función booleana `prime` que tome como parámetro un número natural y devuelva
`true` o `false` dependiendo de si el número es primo o no.

2. Se dice que una palabra es [palíndroma](https://es.wikipedia.org/wiki/Pal%C3%ADndromo) 
si se lee igual de derecha a izquierda que de izquierda a derecha. 
Ejemplos de palíndromas son las palabras "Ana" o "arenera".
Desarrolle una función 
```
bool IsPalindrome(std::string my_string);
```
que determine si la cadena que se le pasa como parámetro es palíndroma o no.
Realice un programa que inicialize un vector de `N` componentes cada una de las cuales sea una cadena
(std::string).
Haga que el programa imprima en pantalla las `N` cadenas del vector, indicando para cada una de ellas si es
palíndroma o no.

3.- La función exponencial, f(x)=e<sup>x</sup>, se puede calcular mediante su desarrollo en 
[serie de Taylor](https://es.symbolab.com/solver/taylor-maclaurin-series-calculator/taylor%20e%5E%7Bx%7D):

![desarrollo en serie de Taylor](https://raw.githubusercontent.com/fsande/-IB-P07-Functions/master/serie.png "Text")

Cuantos más términos tome de la serie, mayor será la precisión de la aproximación a la función.

Diseñe una función 
```
double MyExp(double exponent, unsigned num_terms);
```
que calcule el valor de e<sup>x</sup> para un valor de x que se le pase como parámetro (`exponent`).
El segundo parámetro de la función indica el número de términos del desarrollo en serie de Taylor a utilizar
para el cálculo.

Su función debería utilizar otra función que calcule el factorial de un número que se le pase como parámetro.

Compare los valores que obtiene en su función para diferentes valores del parámetro y compárelos con los que
obtiene al usar la función `exp` definida en el fichero de cabecera `cmath`.

4.- Escriba una función `DiasMes` que reciba como parámetro un número entero que indique el mes (número de 1 a
12) y devuelva el número de días que tiene ese mes.
Si el mes no está en el rango [1, 12] la función debe devolver -1 como resultado.
Suponga que febrero tiene siempre 28 días.
¿Qué cambios habría que hacer a la función para tratar adecuadamente los años bisiestos?.

5.- Un número palíndromo es esquél que permanece igual cuando se invierten sus dígitos. 
Por ejemplo 121 es un número palíndromo mientras que 112 no lo es.
Escriba un programa en C++ que solicite al usuario los límites inferior y superior de un intervalo (`[N, M]`)
y encuentre el número palíndromo más grande y el más pequeño que sean productos de números detro de ese rango.

El programa debería devolver los palíndromos más grandes y más pequeños, junto con los factores de cada uno dentro del rango. 
Si el palíndromo más grande o más pequeño tiene más de un par de factores dentro del rango, entonces devuelve todos los pares.

Ejemplo 1
Dado el intervalo [1, 9] 

Y dada la lista de todos los productos posibles dentro de este rango: 
`[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 14, 16, 18, 15, 21, 24, 27, 20, 28, 32, 36, 25, 30, 35, 40, 45, 42, 48, 54, 49, 56, 63, 64, 72, 81]`
Los productos de palíndromo son todos números de un solo dígito (en este caso): `[1, 2, 3, 4, 5, 6, 7, 8, 9]`.
El palíndromo más pequeño es 1. 
Sus factores son (1, 1). 
El producto de palíndromo más grande es 9. 
Sus factores son (1, 9) y (3, 3).

Ejemplo 2
Dado el rango [10, 99] 
El palíndromo más pequeño es 121. 
Sus factores son (11, 11). 
El producto de palíndromo más grande es 9009. 
Sus factores son (91, 99).

### Referencias
* [Tutorial Fundamentos de Informática](http://www.minidosis.org/#/cursos/FI)
* [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* [La función std::rand](https://en.cppreference.com/w/cpp/numeric/random/rand)
* [La conjetura de Collatz](https://es.wikipedia.org/wiki/Conjetura_de_Collatz) 
* [La clase std::string](http://www.cplusplus.com/reference/string/string/)

