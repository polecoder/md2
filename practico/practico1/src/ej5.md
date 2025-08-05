# Ejercicio 5

## Consigna

Sabiendo que el resto de dividir un entero $a$ por 18 es 5, calcular el resto de:

1. $a^2 - 3a + 11$ al dividir por 18
2. $a^2 + 7$ al dividir por 36
3. $4a + 1$ al dividir por 9
4. $7a^2 + 12$ al dividir por 28

## Resolución

### Parte 1

- $a^2 - 3a + 11$ al dividir por 18

Por el teorema de la división entera, tenemos que:

- $a=18q+5$

Entonces, tenemos que:

$$
\begin{aligned}
&a^2 - 3a + 11\\
&=\scriptstyle{(\text{sustituyendo por }a=18q+5)}\\
&(18q+5)^2-3(18q+5)+11\\
&=\\
&18^2q^2+180q+25-54q-15+11\\
&=\\
&18^2q^2+180q-54q+21\\
&=\\
&18(18q^2+10q-3q)+21\\
&=\\
&18(18q^2+7q+1)+3\\
\end{aligned}
$$

Como $0\leq3<18$ y $18q^2+7q+1\in\mathbb{Z}$, lo llamamos $q'$ y por lo tanto el resto de dividir $a^2 - 3a + 11$ entre $18$ es $3$

### Parte 2

- $a^2 + 7$ al dividir por 36

Por el teorema de la división entera, tenemos que:

- $a=18q+5$

Entonces, tenemos que:

$$
\begin{aligned}
&a^2 + 7\\
&=\scriptstyle{(\text{sustituyendo por }a=18q+5)}\\
&(18q+5)^2+7\\
&=\\
&18^2q^2+180q+25+7\\
&=\\
&18\cdot18q^2+180q+33\\
&=\\
&18\cdot2\cdot9q^2+36\cdot5q+33\\
&=\\
&36\cdot9q^2+36\cdot5q+33\\
&=\\
&36(9q^2+5q)+33\\
\end{aligned}
$$

Como $0\leq33<36$ y $9q^2+5q\in\mathbb{Z}$, lo llamamos $q'$ y por lo tanto el resto de dividir $a^2 + 7$ entre $36$ es $33$

### Parte 4

- $7a^2 + 12$ al dividir por 28

Por el teorema de la división entera, tenemos que:

- $a=18q+5$

Entonces, tenemos que:

$$
\begin{aligned}
&7a^2 + 12\\
&=\scriptstyle{(\text{sustituyendo por }a=18q+5)}\\
&7(18q+5)^2+12\\
&=\\
&7(18^2q^2+180q+25)+12\\
&=\\
&7\cdot2(18\cdot9q^2+90q)+7\cdot25+12\\
&=\\
&7\cdot2\cdot2(9\cdot9q^2+45q)+7\cdot25+12\\
&=\\
&28(9^2q^2+45q)+175+12\\
&=\\
&28(9^2q^2+45q)+189\\
&=\\
&28(9^2q^2+45q)+168+21\\
&=\\
&28(9^2q^2+45q)+28\cdot6+21\\
&=\\
&28(9^2q^2+45q+6)+21\\
\end{aligned}
$$

Como $0\leq21<28$ y $9^2q^2+45q+6\in\mathbb{Z}$, lo llamamos $q'$ y por lo tanto el resto de dividir $7a^2 + 12$ entre $28$ es $21$