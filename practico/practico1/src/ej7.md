# Ejercicio 7

## Consigna

1. Demostrar que el producto de tres naturales consecutivos es múltiplo de 6.
2. Probar que $n(2n + 1)(7n + 1)$ es divisible entre 6 para todo $n \in \mathbb{N}$.

## Resolución

Para este ejercicio vamos a considerar como una prueba suficiente que si un entero es múltiplo de 2 y de 3, entonces también es múltiplo de 6.

### Parte 1

- Demostrar que el producto de tres naturales consecutivos es múltiplo de 6.

Queremos verificar que para todo $n\in\mathbb{N}: n(n+1)(n+2)=6q$ para algún $q\in\mathbb{Z}$. Lo haremos verificando en partes separadas que dicho número es múltiplo de 2 y de 3.

Llamemos $m=n(n+1)(n+2)$.

#### Divisibilidad por 2

- Para todo $n\in\mathbb{N}: n(n+1)(n+2)=2q$ para algún $q\in\mathbb{Z}$

Tenemos los siguientes dos casos posibles para $n$:

- $n=2q$ con $q\in\mathbb{Z}$
- $n=2q+1$ con $q\in\mathbb{Z}$

**CASO 1: $n=2q$**

$$
\begin{aligned}
&n(n+1)(n+2)\\
&=\scriptstyle{(\text{sustituyendo }n=2q)}\\
&2q(2q+1)(2q+2)\\
&=\scriptstyle{(\text{reagrupando})}\\
&2(q(2q+1)(2q+2))\\
\end{aligned}
$$

Y como $q(2q+1)(2q+2)\in\mathbb{Z}$, tenemos que:

- $m=2q'$

Por lo tanto, $m$ es múltiplo de 2 para este caso.

**CASO 2: $n=2q+1$**

$$
\begin{aligned}
&n(n+1)(n+2)\\
&=\scriptstyle{(\text{sustituyendo }n=2q+1)}\\
&(2q+1)(2q+2)(2q+3)\\
&=\scriptstyle{(\text{operando})}\\
&(2q+1)2(q+1)(2q+3)\\
&=\scriptstyle{(\text{reagrupando})}\\
&2(q+1)(2q+1)(2q+3)\\
\end{aligned}
$$

Y como $(q+1)(2q+1)(2q+3)\in\mathbb{Z}$, tenemos que:

- $m=2q'$

Por lo tanto, $m$ es múltiplo de 2 para este caso.

Con esto se concluye que $m$ es múltiplo de 2 en todos los casos. $\square$

#### Divisibilidad por 3

- Para todo $n\in\mathbb{N}: n(n+1)(n+2)=3q$ para algún $q\in\mathbb{Z}$

Tenemos los siguientes dos casos posibles para $n$:

- $n=3q$ con $q\in\mathbb{Z}$
- $n=3q+1$ con $q\in\mathbb{Z}$
- $n=3q+2$ con $q\in\mathbb{Z}$

**CASO 1: $n=3q$**

El caso es directo, de la misma forma que el caso 1 para la divisibilidad entre 2.

**CASO 2: $n=3q+1$**

$$
\begin{aligned}
&n(n+1)(n+2)\\
&=\scriptstyle{(\text{sustituyendo }n=3q+1)}\\
&(3q+1)(3q+2)(3q+3)\\
&=\scriptstyle{(\text{operando})}\\
&(3q+1)(3q+2)3(q+1)\\
&=\scriptstyle{(\text{reagrupando})}\\
&3(q+1)(3q+1)(3q+2)\\
\end{aligned}
$$

Y como $(q+1)(3q+1)(3q+2)\in\mathbb{Z}$, tenemos que:

- $m=3q'$

Por lo tanto, $m$ es múltiplo de 3 para este caso.

**CASO 3: $n=3q+2$**

$$
\begin{aligned}
&n(n+1)(n+2)\\
&=\scriptstyle{(\text{sustituyendo }n=3q+1)}\\
&(3q+2)(3q+3)(3q+4)\\
&=\scriptstyle{(\text{operando})}\\
&(3q+2)3(q+1)(3q+4)\\
&=\scriptstyle{(\text{reagrupando})}\\
&3(q+1)(3q+2)(3q+4)\\
\end{aligned}
$$

Y como $(q+1)(3q+2)(3q+4)\in\mathbb{Z}$, tenemos que:

- $m=3q'$

Por lo tanto, $m$ es múltiplo de 3 para este caso.

Con esto se concluye que $m$ es múltiplo de 3 en todos los casos. $\square$