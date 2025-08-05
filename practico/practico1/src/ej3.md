# Ejercicio 3

## Consigna

El Juego del Polinomio consiste en que alguien elige en secreto un polinomio con coeficientes enteros no negativos y de cualquier grado $n$, es decir:

$$
p(x) = a_n x^n + a_{n-1}x^{n-1} + \dots + a_1 x + a_0, \quad a_i \in \mathbb{N}, \ \forall i
$$

Tenemos que averiguar cuál es el polinomio, pudiendo preguntar cuánto vale $p(x)$ en los valores que deseemos.

1. Considerar una versión simplificada en la que además $0 \leq a_i < 5$ para todo $i$.

    1. Probar que alcanza con conocer $p(5)$ para determinar el polinomio.  
    2. Determinar el polinomio si $p(5) = 89$.

2. Considerar ahora la versión general donde solo sabemos que $a_i \in \mathbb{N}$.

    1. Supongamos que el polinomio es $p(x) = 2x^2 + 7x + 4$. Notar que $p(5) = 89$. ¿Es suficiente conocer $p(5)$ para determinar $p(x)$? ¿Qué cambia respecto al caso anterior?  
    2. Elaborar una estrategia para adivinar cualquier $p$ haciendo la menor cantidad de evaluaciones posibles. Las preguntas pueden hacerse juntas o de forma secuencial.

## Resolución

### Parte 1

Considerar una versión simplificada en la que además $0 \leq a_i < 5$ para todo $i$.

1. Probar que alcanza con conocer $p(5)$ para determinar el polinomio.  
2. Determinar el polinomio si $p(5) = 89$.

#### Subparte 1

- Probar que alcanza con conocer $p(5)$ para determinar el polinomio.  

Veamos que podemos decir sobre la evaluación del polinomio en 5, es decir sobre $p(5)$:

- $p(5)=a_n5^n+a_{n-1}5^{n-1}+\ldots+a_25^2+a_15^1+a_05^0$

Considerando además de esto, que sabemos que los coeficientes cumplen la siguiente propiedad para todo $i: 0\leq a_i<5$, entonces $p(5)$ es la expresión de un número en base 5. 
Por lo que sabiendo el valor de $p(5)$ en base decimal, solo bastaría con convertirlo a la base 5 para obtener el resultado.

- $p(5)=(a_na_{n-1}\ldots a_2a_1a_0)_5$

#### Subparte 2

- Determinar el polinomio si $p(5) = 89$.

Hallemos la expresión en base 5 de 89.

$$
\begin{aligned}
&89=5\cdot17+4\\
&89=5\cdot(5\cdot3+2)+4\\
&89=5^2\cdot3+5^1\cdot2+4\\
&89=(324)_5\\
\end{aligned}
$$

Por lo que se concluye que el polinomio elegido es:

- $p(x)=3x^2+2x+4$

### Parte 2

Considerar ahora la versión general donde solo sabemos que $a_i \in \mathbb{N}$.  

- Supongamos que el polinomio es $p(x) = 2x^2 + 7x + 4$. Notar que $p(5) = 89$. ¿Es suficiente conocer $p(5)$ para determinar $p(x)$? ¿Qué cambia respecto al caso anterior?
- Elaborar una estrategia para adivinar cualquier $p$ haciendo la menor cantidad de evaluaciones posibles. Las preguntas pueden hacerse juntas o de forma secuencial.

#### Subparte 1

- Supongamos que el polinomio es $p(x) = 2x^2 + 7x + 4$. Notar que $p(5) = 89$. ¿Es suficiente conocer $p(5)$ para determinar $p(x)$? ¿Qué cambia respecto al caso anterior?

Para esta parte, cambia algo muy importante, y es que si hay algún coeficiente mayor o igual a 5, el polinomio ya no será $p(5)$ expresado en base 5. El ejemplo que se muestra es claro.
En cambio, si hubieramos elegido un número mayor al máximo coeficiente, por ejemplo 8, ahí si nos bastaría con conocer $p(8)$, por el mismo razonamiento que hicimos en la parte 1.

- $p(8)=(274)_8$

#### Subparte 2

- Elaborar una estrategia para adivinar cualquier $p$ haciendo la menor cantidad de evaluaciones posibles. Las preguntas pueden hacerse juntas o de forma secuencial.

Bueno, para esta parte tenemos que basarnos fuertemente en los requerimientos que nos deja en análisis que hicimos en la subparte 1. Necesitamos encontrar un número que sea más grande que todos los coeficientes, entonces preguntamos por la siguiente evaluación:

1. ¿Cuánto vale $p(1)$?

Ya que con esto, sabremos el valor de la suma de todos los coeficientes, pues:

- $p(1)=a_n\cdot1^n+\ldots+a_1\cdot1^1+a_0\cdot1^0=a_n+\ldots+a_1+a_0$
- Llamamos $m$ al valor de $p(1)$ 

Y con esto ya estamos preparados para realizar la última pregunta que nos permite encontrar el poliniomio y es:

2. ¿Cuánto vale $p(m+1)$?

Y una vez que tenemos esta respuesta, podremos aplicar nuevamente los conceptos que utilizamos en la parte 1.