# Ejercicio 6

## Consigna

Sean $a,\ b,\ c,\ d \in \mathbb{N}$. Probar o refutar (dando contraejemplos) las siguientes afirmaciones:

1. Si $a \mid b$ y $c \mid d$ entonces $ac \mid bd$  
2. Si $a \mid b$ entonces $ac \mid bc$  
3. Si $a \nmid bc$ entonces $a \nmid b$ y $a \nmid c$  
4. Si $ac \mid bc$ entonces $a \mid b$  
5. Si $a \mid bc$ entonces $a \mid b$ o $a \mid c$  
6. Si $a \mid c$ y $b \mid c$ entonces $ab \mid c$  
7. Si $4 \mid a^2$ entonces $2 \mid a$  
8. Si $9 \mid b + c$ entonces $9 \mid b$ o $9 \mid c$  
9. Si $a + c \mid b + c$ entonces $a \mid b$

## Resolución

### Parte 1

- Si $a \mid b$ y $c \mid d$ entonces $ac \mid bd$

Por el teorema de la división entera, tenemos que:

1. $a\mid b\to b=aq$ con $q\in\mathbb{Z}\quad(*_1)$
2. $c\mid d\to d=cq'$ con $q'\in\mathbb{Z}\quad(*_2)$

Queremos probar que:

- $ac\mid bd$, que es equivalente a decir que:
- $bd=acq''$ con $q''\in\mathbb{Z}$

Por las hipótesis $(*_1),(*_2)$

$$
\begin{aligned}
&bd=acq''\\
&\iff\scriptstyle{(\text{sustituyendo por las hipótesis})}\\
&aqcq'=acq''\\
&\iff\scriptstyle{(\text{operatoria})}\\
&qq'=q''\\
\end{aligned}
$$

Como $q''\in\mathbb{Z}$ (pues es el producto de dos enteros), queda demostrado que $ac\mid bd$

Por lo tanto esta afirmación es VERDADERA.

### Parte 2

- Si $a \mid b$ entonces $ac \mid bc$

Por el teorema de la división entera, tenemos que:

1. $a\mid b\to b=aq$ con $q\in\mathbb{Z}\quad(*_1)$

Queremos probar que:

- $ac\mid bc$, que es equivalente a decir que:
- $bc=acq'$ con $q'\in\mathbb{Z}$

Por la hipótesis $(*_1)$ tenemos que:

$$
\begin{aligned}
&bc=acq'\\
&\iff\scriptstyle{(\text{sustituyendo por la hipótesis})}\\
&aqc=acq'\\
&\iff\scriptstyle{(\text{operatoria})}\\
&q=q'\\
\end{aligned}
$$

Como $q'\in\mathbb{Z}$, queda demostrado que $ac\mid bc$.

Por lo tanto esta afirmación es VERDADERA.

### Parte 3

- Si $a \nmid bc$ entonces $a \nmid b$ y $a \nmid c$ 

Para esta parte, asumimos la hipótesis, y suponemos que $a\mid b$. Por el teorema de la división entera tenemos que:

- $a\mid b\to b=aq$ con $q\in\mathbb{Z}$

A partir de esto tenemos que:

$$
\begin{aligned}
&b=aq\\
&\iff\\
&bc=aqc\\
\end{aligned}
$$

Donde considerando $q'=qc\in\mathbb{Z}$, tenemos que $a\mid bc$, lo cual es ABSURDO.

Por lo tanto esta afirmación es VERDADERA.

### Parte 4

- Si $ac \mid bc$ entonces $a \mid b$

Por el teorema de la división entera, tenemos que:

1. $ac\mid bc\to bc=acq$ con $q\in\mathbb{Z}\quad(*_1)$

Queremos probar que:

- $a\mid b$, que es equivalente a decir que:
- $b=aq'$ con $q'\in\mathbb{Z}$

Por la hipótesis $(*_1)$ tenemos que:

$$
\begin{aligned}
&bc=acq\\
&\iff\scriptstyle{(\text{considerando }c\neq0)}\\
&b=aq\\
\end{aligned}
$$

Entonces en este caso, considerando $q'=q\in\mathbb{Z}$, tenemos que la propiedad es verdadera.

Faltaría verificar el caso en el que $c=0$, pero este es trivial, pues el antecedente sería falso:

- $a0\nmid b0$ pues 0 no divide a ningún número.

Por lo tanto esta afirmación es VERDADERA.

### Parte 5

- Si $a \mid bc$ entonces $a \mid b$ o $a \mid c$

Consideremos $a=6,b=3,c=4$. Entonces:

- $6\mid12$, pero:
- $6\nmid3$ ni
- $6\nmid4$

Por lo que esta afirmación es FALSA.

### Parte 6

- Si $a \mid c$ y $b \mid c$ entonces $ab \mid c$

Consideremos $a=4,b=2,c=4$. Entonces:

- $4\mid4$ y $2\mid4$, pero
- $8\nmid4$

Por lo que esta afirmación es FALSA.

