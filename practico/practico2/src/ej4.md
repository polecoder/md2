# Ejercicio 4

## Consigna

Sean $a, b, c \in \mathbb{N}$. Probar las siguientes afirmaciones:

1. $mcd(ca, cb) = c \cdot mcd(a, b)$.  *Sugerencia: usar Bezout y probar la doble desigualdad.*
2. Si $c \mid a$ y $c \mid b$ entonces:  

    - $mcd(\frac{a}{c}, \frac{b}{c}) = \frac{mcd(a, b)}{c}$

3. Si $a$ y $b$ son primos entre sí, entonces:

    - $mcd(a - b, a + b) = 1$ o $2$

    *Sugerencia: probar primero que $mcd(a - b, a + b)$ divide a $mcd(2a, 2b)$.*

## Resolución

### Parte 1

- $mcd(ca, cb) = c \cdot mcd(a, b)$

La estrategia será probar las dos desigualdades, por lo que vamos a empezar con eso.
Llamemos:

- $d=mcd(a,b)$
- $d'=mcd(ca,cb)$

#### $d'\leq cd$

Veamos el siguiente razonamiento usando Bézout:

$$
\begin{aligned}
&d=ax+by\\
&\iff\scriptstyle{(\text{multiplico por c})}\\
&cd=cax+cby\\
&\iff\scriptstyle{(ca=d'q_1;cb=d'q_2\text{ con }q_1,q_2\in\mathbb{Z})}\\
&cd=cax+cby\\
&\iff\\
&cd=d'q_1x+d'q_2y\\
&\iff\\
&cd=d'(q_1x+q_2y)\\
&\iff\scriptstyle{((q_1x+q_2y)\in\mathbb{Z})}\\
&d'\mid cd\\
&\iff\\
&d'\leq cd
\end{aligned}
$$

#### $cd\leq d'$

Veamos el siguiente razonamiento usando Bézout:

$$
\begin{aligned}
&d'=cax+cby\\
&\iff\scriptstyle{(a=dq_1;b=dq_2\text{ con }q_1,q_2\in\mathbb{Z})}\\
&d'=cdq_1x+cdq_2y\\
&\iff\\
&d'=cd(q_1x+q_2y)\\
&\iff\scriptstyle{((q_1x+q_2y)\in\mathbb{Z})}\\
&cd\mid d'\\
&\iff\\
&cd\leq d'\\
\end{aligned}
$$

Juntando las dos partes, tenemos lo que queríamos probar:

- $d'=cd$

### Parte 2

- Si $c \mid a$ y $c \mid b$ entonces:  

    - $mcd(\frac{a}{c}, \frac{b}{c}) = \frac{mcd(a, b)}{c}$

La estrategia será probar las dos desigualdades, por lo que vamos a empezar con eso.
Llamemos:

- $d=mcd(a,b)$
- $d'=mcd(\frac{a}{c},\frac{b}{c})$

#### $d'\leq \frac{d}{c}$

Veamos el siguiente razonamiento usando Bézout:

$$
\begin{aligned}
&d=ax+by\\
&\iff\scriptstyle{(\text{dividiendo por }c\neq0)}\\
&\frac{d}{c}=\frac{a}{c}x+\frac{b}{c}y\\
&\iff\scriptstyle{(\frac{a}{c}=d'q_1;\frac{b}{c}=d'q_2\text{ con }q_1,q_2\in\mathbb{Z})}\\
&\frac{d}{c}=d'q_1x+d'q_2y\\
&\iff\\
&\frac{d}{c}=d'(q_1x+q_2y)\\
&\iff\scriptstyle{(\text{como }(q_1x+q_2y)\in\mathbb{Z})}\\
&d'\mid\frac{d}{c}\\
&\iff\\
&d'\leq\frac{d}{c}\\
\end{aligned}
$$

#### $\frac{d}{c}\leq d'$

Veamos el siguiente razonamiento usando Bézout:

$$
\begin{aligned}
&d'=\frac{a}{c}x+\frac{b}{c}y\\
&\iff\scriptstyle{(a=dq_1;b=dq_2\text{ con }q_1,q_2\in\mathbb{Z})}\\
&d'=\frac{d}{c}q_1x+\frac{d}{c}q_2y\\
&\iff\\
&d'=\frac{d}{c}(q_1x+q_2y)\\
&\iff\scriptstyle{(\text{como }(q_1x+q_2y)\in\mathbb{Z})}\\
&\frac{d}{c}\mid d'\\
&\iff\\
&\frac{d}{c}\leq d'
\end{aligned}
$$

- $d'=\frac{d}{c}$

### Parte 3

- Si $a$ y $b$ son primos entre sí, entonces:

    - $mcd(a - b, a + b) = 1$ o $2$

    *Sugerencia: probar primero que $mcd(a - b, a + b)$ divide a $mcd(2a, 2b)$.*

Como indica la sugerencia, primero probaremos lo que se indica. Es decir:

- $mcd(a-b,a+b)\mid mcd(2a,2b)$

Llamamos:

- $d=mcd(a-b,a+b)$

Usaremos el siguiente corolario de la igualdad de Bézout:

- Dado $e\in\mathbb{Z}$, si $e\mid a$ y $e\mid b$, entonces $e\mid mcd(a,b)$

Por lo tanto queremos probar que:

1. $d\mid 2a$
2. $d\mid 2b$

Como tenemos que $d\mid a-b$ y $d\mid a+b$ concluimos que:

1. $d\mid1(a-b)+1(a+b)\to d\mid 2a$
2. $d\mid(-1)(a-b)+1(a+b)\to d\mid 2b$

Concluimos entonces que:

- $d\mid mcd(2a,2b)$

Con esto, retornamos a la propiedad original que queremos probar, es decir que:

- $mcd(a - b, a + b) = 1$ o $2$

Veamos el siguiente razonamiento:

$$
\begin{aligned}
&mcd(2a,2b)\\
&=\scriptstyle{(\text{parte 1 del ejercicio})}\\
&2mcd(a,b)\\
&=\scriptstyle{(\text{hipótesis})}\\
&2\\
\end{aligned}
$$

Y cómo $mcd(a-b,a+b)\mid mcd(2a,2b)=2$, necesariamente tenemos las dos opciones:

- $mcd(a-b,a+b)=1$, o
- $mcd(a-b,a+b)=2$

Lo que demuestra la propiedad.