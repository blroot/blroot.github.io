---
published: true
---
Propiedades de integral definida, Función integral, Teorema fundamental del cálculo integral, Regla de Barrow, Cálculo de área, Área entre curvas.

## Integral indefinida

### Propiedades

1- $$ \int_a^b c*dx = c * \int_a^b dx = c(b-a) $$

2- $$ \int_a^b [f(x)*dx+g(x)*dx]*dx = \int_a^b f(x)*dx + \int_a^b g(x)*dx $$

3- $$ \int_a^a f(x)*dx = 0 $$

4- $$ \int_a^b f(x)*dx = - \int_b^a f(x)*dx $$

5- Sea $f$ continua en $[a,b] \implies f$ es integrable en $[a,b]$ 

$$ \implies \exists \int_a^b f(x)*dx \in R$$

6- Sea $f$ continua y $c \in [a,b]$

$$\implies \int_a^b f(x)*dx = \int_a^c f(x)*dx + \int_c^b f(x)*dx$$

7- Sea $f(x) \le g(x) \forall x \in [a,b]$
$$\implies \int_a^b f(x)*dx \le \int_a^b g(x)*dx$$

### Función integral

Si alguno de los extremos en la integral definida es variable, será una función integral.

Ej:

$$ \int_a^(B(x)) f(t)*dt $$

### Teorema fundamental del cálculo integral

Sea $f(x)$ una función continua en $[a,b]$ y sea $g(x) = \int_a^x f(t)*dt$

$\implies g'(x)=(\int_a^x f(t)*dt)'=f(x)$

Es decir, se puede comprender a la integración y a la derivación como operaciones inversas.

### Regla de Barrow

Sea f(x) continua en $[a,b]$ y sea:

$$ \int_a^b f(x)*dx = P(x)+C \biggr ]_a^b = (P(b)+C)-(P(a)+C) = P(b)-P(a) $$

### Área de figuras planas

Para que el cálculo de área tenga sentido, ésta debe ser positiva, por lo tanto, sea $f(x)$ una función continua en $[a,b]$, para calcular el área de dicha curva entre $x=a$ y $x=b$ y el éje de abscisas:

$$ \int_a^b |f(x)|*dx $$

### Área entre curvas

Para hallar el área entre las curvas de dos funciones $f(x)$ y $g(x)$, hay que intregar $f(x)-g(x)$ en los intervalos en donde $f(x)>g(x)$, por el contrario, hay que integrar $g(x)-f(x)$ en los intervalos en que $g(x)>f(x)$



