---
published: true
---
Integral doble, teorema de Fubini, integrales dobles sobre regiones más generales, cálculo de una región , integrales dobles por cambio de variables, cambio a coordenadas polares.

## Integral Doble

En las integrales dobles tenemos dos variables, esto implica que con respecto a la integración en una variable va a variar la región sobre la cual integramos, cuya a forma geométrica elemental va a ser un rectángulo o cuadrado:

De forma iterada:

$$ I = \int_{y=c}^{y=d} ( \int_{x=a}^{x=b} f(x,y)dx)dy $$

## Teorema de Fubini

Dicho teorema demuestra que  (1) también se puede calcular invirtiendo el órden de integración

Ejemplo:

Calcular $$\int_R x^2ydxdy$$ siendo $$R$$ la región definida por $$0 \le x \le 1; 0 \le y \le 3$$

$$ I = \int_{y=0}^{y=3} (\int_{x=0}^{x=1} x^2ydx)dy = \int_{0}^{3} [y \frac{x^3}{3}]_0^1 dy \\
= \frac{1}{3} \int_{0}^{3} ydy = \frac{3}{2} 
$$
