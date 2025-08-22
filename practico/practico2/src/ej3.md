# Ejercicio 3

## Consigna

Sean $a, b, c \in \mathbb{N}$ tales que $mcd(a, b) = 1$ (a y b son primos entre sí). Probar o dar un contraejemplo de las siguientes afirmaciones:

1. Si $a \mid (bc)$ entonces $a \mid c$ 
2. Si $a \mid c$ y $b \mid c$ entonces $ab \mid c$.
3. ¿Valen las partes anteriores si $mcd(a, b) \neq 1$?

## Resolución

### Parte 1

- Si $a \mid (bc)$ entonces $a \mid c$ 

Como $mcd(a,b)=1$, por Bézout tenemos que:

- $\exists x,y\in\mathbb{Z}$ tales que $ax+by=1$, múltiplicando la expresión por $c$ tenemos que:

- $cax+cby=c$

Veamos el siguiente razonamiento, basándonos en que $a\mid bc$:

$$
\begin{aligned}
&cax+cby=c\\
&\iff\scriptstyle{(bc=\dot{a}\text{, es decir }bc=az\text{ con }z\in\mathbb{Z})}\\
&cax+azy=c\\
&\iff\\
&a(cx+zy)=c\\
\end{aligned}
$$

Como $cx+zy\in\mathbb{Z}$ tenemos que $c=\dot{a}$ que es lo que queríamos probar.

### Parte 2

- Si $a \mid c$ y $b \mid c$ entonces $ab \mid c$

Por hipótesis tenemos que:

- $c=aq_1$ con $q_1\in\mathbb{Z}$
- $c=bq_2$ con $q_2\in\mathbb{Z}$

Veamos el siguiente razonamiento entonces:

$$
\begin{aligned}
&c^2=aq_1bq_2\\
&\iff\\
&c^2=ab(q_1q_2)\\
&\iff\scriptstyle{(\text{como }q_1q_2\in\mathbb{Z})}\\
&c^2=ab(q_1q_2)\\
&\iff\\
&ab\mid c^2\\
&\iff\scriptstyle{(\text{por el lema de Euclides})}\\
&ab\mid c\\
\end{aligned}
$$

Por lo que esto prueba la propiedad.

### Parte 3

- Valen las partes anteriores si $mcd(a, b) \neq 1$?

#### Parte 1

- Si $a \mid (bc)$ entonces $a \mid c$ 

Veamos un contraejemplo considerando:

- $a=4$
- $b=6$
- $c=2$

Entonces la propiedad sería: "Si $4\mid 12$ entonces $4\mid 2$".
Esto es claramente falso, pues $4\nmid 2$.

#### Parte 2

- Si $a \mid c$ y $b \mid c$ entonces $ab \mid c$

Veamos un contraejemplo considerando:

- $a=2$
- $b=4$
- $c=4$

Entonces la propiedad sería: "Si $2\mid4$ y $4\mid4$ entonces $8\mid4$"
Esto es claramente falso, pues $8\nmid4$