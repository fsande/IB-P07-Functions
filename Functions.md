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





### Referencias
* [Tutorial Fundamentos de Informática](http://www.minidosis.org/#/cursos/FI)
* [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* [La función std::rand](https://en.cppreference.com/w/cpp/numeric/random/rand)
* [La conjetura de Collatz](https://es.wikipedia.org/wiki/Conjetura_de_Collatz) 
* [La clase std::string](http://www.cplusplus.com/reference/string/string/)

