# Taller-2

Pseudocodigo
function convertirABooleana(n):
    if n == 0:
        return "0"
    else:
        return convertirABooleana(n // 2) + str(n % 2)

Explicación del Pseudocódigo:

La función convertirABooleana toma un número natural ( n ) como entrada.
Si ( n ) es 0, la función retorna “0”.
Si ( n ) no es 0, la función llama recursivamente a convertirABooleana con el cociente de ( n ) dividido por 2 y concatena el residuo de ( n ) dividido por 2 (0 o 1) al resultado de la llamada recursiva.


Descripción del Algoritmo
Descripción del problema: Dado un número natural ( n ), calcular su representación booleana.

Estrategia “Dividir y Vencer”: La estrategia “dividir y vencer” consiste en descomponer un problema grande en subproblemas más pequeños, resolver cada subproblema de manera recursiva y luego combinar las soluciones de los subproblemas para obtener la solución del problema original.

Pasos del Algoritmo:

Dividir: Dividir el número ( n ) por 2.
Vencer: Obtener el residuo de la división (0 o 1) y almacenar el cociente.
Combinar: Repetir el proceso con el cociente hasta que sea 0. La representación booleana será la concatenación de los residuos en orden inverso.

Análisis Experimental
Se midió el tiempo de ejecución del algoritmo para valores de ( n ) desde 1 hasta 30000. Los resultados muestran que el tiempo de ejecución es lineal respecto al tamaño del número, lo cual es esperado dado que cada llamada recursiva reduce el tamaño del problema a la mitad.