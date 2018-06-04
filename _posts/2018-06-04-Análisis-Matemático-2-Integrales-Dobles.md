---
published: true
---
Integral doble, teorema de Fubini, integrales dobles sobre regiones generales, cálculo del área de una región, integrales dobles por cambio de variables, cambio a coordenadas polares.

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

## Integrales dobles sobre regiones generales

Como es de esperarse, en dos variables vamos a querer integrar funciones sobre regiones $$D$$ más generales que un rectángulo o cuadrado, vamos a definir dos tipos de regiones:

### Región tipo 1

Se dice que una región plana $$D$$ es de tipo 1 si yace entre las gráficas de dos funciones continuas de $$x$$:

$$D = (x,y) \in \Re^2 / a \le x \le b, g_{1}(x) \le y \le g_{2}(x)$$

luego, $$ I = \int\int_{D} f(x,y) dA = \int_{a}^{b} \int_{y=g_{1}(x)}^{y=g_{2}(x)} f(x,y)dy dx $$

### Región tipo 2

Se dice que una región plana $$D$$ es de tipo 1 si yace entre las gráficas de dos funciones continuas de $$y$$:

$$D = (x,y) \in \Re^2 / c \le y \le d, h_{1}(y) \le y \le h_{2}(y)$$

luego, $$ I = \int\int_{D} f(x,y) dA = \int_{c}^{d} \int_{x=h_{1}(y)}^{x=h_{2}(y)} f(x,y)dx dy $$

En algunos casos, vamos a encontrar que se puede expresar una región como tipo 1 y también como tipo 2 haciendo la correspondiente inversa de las funciones que acotan la región (lo cual no siempre es fácil o conveniente.

## Cálculo del área de una región

Cuando la función que integramos es un escalar igual a 1, la integral doble da como resultado el área de la región $$R$$

Ejemplo:

Calcular el área limitada entre la curva de ecuación: $$x+2y^2-8=0$$ y el eje $$y$$

Como una región de tipo 2:

$$ A = \int_{-2}^{2} (\int_{0}^{8-2y^2} 1 dx)dy = \int_{-2}^{2} ([x]_0^{8-2y^2})dy \\
\int_{-2}^{2} (8-2y^2)dy = [8y-2 \frac{y^3}{3}]_-2^2 = \frac{64}{3}
$$


