# Ejercicio 1

## Consigna

1. Escribir en las bases 2, 4, 8 y 16 los números decimales: 137, 6243 y 12354.
2. Escribir en la base 28 el número decimal 16912.
3. Escribir en las bases 2 y 10 los números hexadecimales: A7, 4C2, 1C2B y A2DFE.
4. Escribir en las bases 10 y 16 los números binarios: 11001110, 00110001, 11110000 y 01010111.
5. Pasar los siguientes números, dados en las bases indicadas, a decimal: $(BACK)_{21}$ y $(OJO)_{25}$.

## Resolución

### Parte 1

- $137$:
    - Base 2:
        $$
        \begin{aligned}
        &137=2\times68+1\\
        &137=2\times(2\times34+0)+1\\
        &137=2\times(2\times(2\times17+0)+0)+1\\
        &137=2\times(2\times(2\times(2\times8+1)+0)+0)+1\\
        &137=2\times(2\times(2\times(2\times(2\times4+0)+1)+0)+0)+1\\
        &137=2\times(2\times(2\times(2\times(2\times(2\times2+0)+0)+1)+0)+0)+1\\
        &137=2^7+2^3+2^0\\
        &137=(10001001)_2
        \end{aligned}
        $$
    - Base 4:
        $$
        \begin{aligned}
        &137=2^7+2^3+2^0\\
        &137=4\cdot2^5+4\cdot2+4^0\\
        &137=4^2\cdot2^3+4\cdot2+4^0\\
        &137=4^3\cdot2+4\cdot2+4^0\cdot1\\
        &137=(2021)_4
        \end{aligned}
        $$
    - Base 8:
        $$
        \begin{aligned}
        &137=2^7+2^3+2^0\\
        &137=2^3\cdot2^4+2^3+2^0\\
        &137=2^6\cdot2+2^3+2^0\\
        &137=8^2\cdot2+8\cdot1+8^0\\
        &137=(211)_8
        \end{aligned}
        $$
    - Base 16:
        $$
        \begin{aligned}
        &137=4^3\cdot2+4\cdot2+4^0\cdot1\\
        &137=4^2\cdot4\cdot2+8+1\\
        &137=16\cdot8+9\\
        &137=(89)_{16}
        \end{aligned}
        $$

- $12354$:
    - Base 16:
        $$
        \begin{aligned}
        &12354=16\cdot772+2\\
        &12354=16\cdot(16\cdot48+4)+2\\
        &12354=16\cdot(16\cdot(16\cdot3+0)+4)+2\\
        &12354=16^3\cdot3+16^2\cdot0+16^1\cdot4+16^0\cdot2\\
        &12354=(3042)_{16}
        \end{aligned}
        $$
    - Base 4:
        $$
        \begin{aligned}
        &12354=16^3\cdot3+16^2\cdot0+16^1\cdot4+16^0\cdot2\\
        &12354=4^6\cdot3+4^4\cdot0+4^2\cdot4+4^0\cdot2\\
        &12354=4^6\cdot3+4^3+4^0\cdot2\\
        &12354=(3001002)_4
        \end{aligned}
        $$
    - Base 2:
        $$
        \begin{aligned}
        &12354=4^6\cdot3+4^3+4^0\cdot2\\
        &12354=2^{12}\cdot3+2^6+2^0\cdot2\\
        &12354=2^{12}\cdot(2+1)+2^6+2^1\\
        &12354=2^{13}+2^{12}+2^6+2^1\\
        &12354=(11000001000010)_2
        \end{aligned}
        $$
    - Base 8:
        $$
        \begin{aligned}
        &12354=2^{13}+2^{12}+2^6+2^1\\
        &12354=2^{12}\cdot2+2^{12}+2^6+2^1\\
        &12354=8^4\cdot2+8^4+8^2+2\\
        &12354=8^4\cdot3+8^2+8^0\cdot2\\
        &12354=(30102)_8\\
        \end{aligned}
        $$

Para esta parte, lo más simple es utilizar las representaciones de una base potencia de dos para ir representando otras.

### Parte 3

- Escribir en las bases 2 y 10 los números hexadecimales: A7, 4C2, 1C2B y A2DFE.

- $(A7)_{16}:$

    - Base 10:
        $$
        \begin{aligned}
        &(A7)_{16}=16^1\cdot10+16^0\cdot7\\
        &(A7)_{16}=167\\
        \end{aligned}
        $$
    - Base 2:
        $$
        \begin{aligned}
        &(A7)_{16}=16^1\cdot10+16^0\cdot7\\
        &(A7)_{16}=2^4\cdot10+2^0\cdot7\\
        &(A7)_{16}=2^4\cdot(2^3+2^1)+2^0\cdot(2^2+3)\\
        &(A7)_{16}=2^7+2^5+2^2+2^1+1\\
        &(A7)_{16}=2^7+2^5+2^2+2^1+2^0\\
        &(A7)_{16}=(10100111)_2
        \end{aligned}
        $$

- $(4C2)_{16}$:
    - Base 10:
        $$
        \begin{aligned}
        &(4C2)_{16}=16^2\cdot4+16\cdot12+2\\
        &(4C2)_{16}=1218
        \end{aligned}
        $$

    - Base 2:
        $$
        \begin{aligned}
        &(4C2)_{16}=16^2\cdot4+16\cdot12+2\\
        &(4C2)_{16}=2^8\cdot4+2^4\cdot12+2\\
        &(4C2)_{16}=2^8\cdot2^2+2^4\cdot(2^3+4)+2^1\\
        &(4C2)_{16}=2^8\cdot2^2+2^4\cdot(2^3+2^2)+2^1\\
        &(4C2)_{16}=2^{10}+2^7+2^6+2^1\\
        &(4C2)_{16}=(10011000010)_2\\
        \end{aligned}
        $$
