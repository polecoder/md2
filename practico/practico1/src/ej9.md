# Ejercicio 9

## Consigna

Probar que las siguientes afirmaciones son verdaderas para todo $n \in \mathbb{N}$:

1. $99 \mid 10^{2n} + 197$
2. $9 \mid 7 \cdot 5^{2n} + 2^{4n+1}$
3. $56 \mid 13^{2n} + 28n^2 - 84n - 1$
4. $256 \mid 7^{2n} + 208n - 1$

## Resolución

La estrategia para este tipo de ejercicios es usar inducción completa.

### Parte 1

- $P(k):10^{2k}+197$

#### Paso base

- $n=0:99\mid10^0+197$

Ese caso es trivial pues:

$$
\begin{aligned}
&10^0+197\\
&=\\
&198\\
&=\\
&99\cdot2
\end{aligned}
$$

Por lo tanto la propiedad es válida para $n=0$

#### Paso inductivo

- (HI): $P(k): 10^{2k}+197$
- (TI): $P(k+1): 10^{2(k+1)}+197$

De la hipótesis, podemos llegar a que:

- $10^{2k}+197=99m$ para algún $m\in\mathbb{Z}$, y por tanto:
- $10^{2k}=99m-197\quad(*_1)$

Expandamos la tesis inductiva para ver si podemos utilizar la hipótesis inductiva:

$$
\begin{aligned}
&10^{2(k+1)}+197\\
&=\scriptstyle{(\text{operando})}\\
&10^{2k+2}+197\\
&=\scriptstyle{(\text{operando})}\\
&10^{2k}10^2+197\\
&=\scriptstyle{(\text{usando la observación }(*_1))}\\
&(99m-197)100+197\\
&=\scriptstyle{(\text{operando})}\\
&100\cdot99m-100\cdot197+197\\
&=\scriptstyle{(\text{operando})}\\
&100\cdot99m-99\cdot197\\
&=\scriptstyle{(\text{sacando factor común})}\\
&99(100m-197)
\end{aligned}
$$

Y considerando que $100m-197\in\mathbb{Z}$, concluimos que $10^{2(k+1)}+197$ es múltiplo de 99, lo cual demuestra la propiedad por inducción. $\square$

### Parte 2

- $P(k):9\mid7\cdot5^{2k}+2^{4k+1}$

#### Paso base

- $n=0:9\mid7\cdot5^{0}+2^{0+1}$

Ese caso es trivial pues:

$$
\begin{aligned}
&7\cdot5^{0}+2^{0+1}\\
&=\\
&7+2\\
&=\\
&9\cdot1
\end{aligned}
$$

Por lo tanto la propiedad es válida para $n=0$

#### Paso inductivo

- (HI): $P(k):9\mid7\cdot5^{2k}+2^{4k+1}$
- (TI): $P(k+1):9\mid7\cdot5^{2(k+1)}+2^{4(k+1)+1}$

De la hipótesis, podemos llegar a que:

- $7\cdot5^{2k}+2^{4k+1}=9m$ para algún $m\in\mathbb{Z}$, y por tanto:
- $2^{4k+1}=9m-7\cdot5^{2k}\quad(*_1)$

Expandamos la tesis inductiva para ver si podemos utilizar la hipótesis inductiva:

$$
\begin{aligned}
&7\cdot5^{2(k+1)}+2^{4(k+1)+1}\\
&=\scriptstyle{(\text{operando})}\\
&7\cdot5^{2k+2}+2^{4k+5}\\
&=\scriptstyle{(\text{operando})}\\
&7\cdot5^{2k}5^2+2^{4k+1}2^4\\
&=\scriptstyle{(\text{usando la observación }(*_1))}\\
&7\cdot5^{2k}5^2+(9m-7\cdot5^{2k})2^4\\
&=\scriptstyle{(\text{operando})}\\
&7\cdot5^{2k}5^2+9m2^4-7\cdot5^{2k}2^4\\
&=\scriptstyle{(\text{operando})}\\
&7\cdot5^{2k}(5^2-2^4)+9m2^4\\
&=\scriptstyle{(\text{operando})}\\
&7\cdot5^{2k}(9)+9m2^4\\
&=\scriptstyle{(\text{sacando factor común})}\\
&9(7\cdot5^{2k}+m2^4)\\
\end{aligned}
$$

Y considerando que $7\cdot5^{2k}+m2^4\in\mathbb{Z}$, concluimos que $7\cdot5^{2(k+1)}+2^{4(k+1)+1}$ es múltiplo de 9, lo cual demuestra la propiedad por inducción. $\square$