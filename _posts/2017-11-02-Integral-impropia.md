---
published: true
---
I.I de primera especie, I.I de segunda especie, criterio de convergencia para funciones no negativas, criterio de límite.

### Integral indefinida de primera especie

Sea $f:[a, + \inf)->R / f$ es integrable en $[a, t] \forall t \in [a, + \inf)$ y sea f acotada.
Si consideramos la función integral :

$$g(x)= \int_a^x f(t)*dt$$

al par $(f;g)$ se lo llama integral impropia de primera especie y se nota 

$$\int_a^{+ \inf} f(x)*dx$$

Se dice que al calcular 

$$\lim_{x\to + \inf} \int_a^b f(x)*dx = \lim {x\to + \inf} g(b) = L$$

1- Si $L \in R \implies$ Converge (C.V)

2- Si $L= \pm inf \implies$ Diverge (D.V)

3- Si $\nexists L \implies$ Oscila

Ej:

$$ \int_0^{+ \inf} 1/(1+x^2)*dx = \lim_{b\to + \inf} \int_0^b 1/(1+x^2)*dx = \lim_{b\to + \inf} \biggr [ arctg \biggr ]_0^b \\
= \lim_{b\to + \inf} arctg(b)-arctg(0) = pi/2 \implies I.I converge
$$

### Integral indefinida de segunda especie

Sea $f:[a, b)->R / f$ es integrable $\forall t \in [a, t)$ con $t \in [a,b)$ y sea f no acotada.
Si consideramos la función integral:

$$g(x)= \int_a^x f(t)*dt$$

al par $(f;g)$ se lo llama integral impropia de segunda especie y se nota 

$$\int_a^{-b} f(x)*dx$$

Si al calcular 

$$ \lim_{t\to b-} \int_a^t f(x)*dx = L $$

1- Si $L \in R \implies$ Converge (C.V)

2- Si $L= \pm inf \implies$ Diverge (D.V)

3- Si $\nexists L \implies$ Oscila

Ej:

$$ \int_{0+}^1 1/x*dx = \lim_{a\to 0+} \int_a^1 1/x*dx = \lim_{a\to 0+} \biggr [ ln|x| \biggr ]_a^1 \\
= \lim_{a\to 0+} ln|1|-ln|a| = +inf \implies $$ I.I diverge

### Criterio de convergencia para funciones no negativas

Sean $f,g:[a,b)->r$ funciones no negativas de primera o segunda especie, integrables en $[a,t] \forall t \in (a,b) / 0 < f(x) < g(x)$

1- Si $$\int_a^{b-} g(x)*dx$$ C.V. $$\implies \int_a^{b-} f(x)*dx$$ C.V.

2- Si $$\int_a^{b-} g(x)*dx$$ D.V. $$\implies \int_a^{b-} f(x)*dx$$ D.V.






