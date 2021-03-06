---
published: true
---
Integral doble, teorema de Fubini, integrales dobles sobre regiones generales, cálculo del área de una región, integrales dobles por cambio de variables, cambio a coordenadas polares.

## Integral Doble

En las integrales dobles tenemos dos variables, esto implica que con respecto a la integración en una variable va a variar la región sobre la cual integramos, pasamos de integrar sobre un intervalo a integrar sobre una región:

La forma más elemental de dicha región es un rectángulo o cuadrado.

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
\int_{-2}^{2} (8-2y^2)dy = [8y-2 \frac{y^3}{3}]_{-2}^2 = \frac{64}{3}
$$

## Integrales dobles por cambio de variables

En muchos casos al igual que en una variable, es útil hacer un cambio de variables para simplificar el cálculo de la integral.
En dos variables, hacer un cambio de variables implica hacer una transformación de una región general a un rectángulo y viceversa.

Sea $$R_{xy}$$ una región general, si aplicamos un cambio de variables por $$u,v$$:

$$
\left\{\begin{aligned}
&u=u(x,y) \\
&v=v(x,y)
\end{aligned}
\right.
$$

Vamos a presentar dos casos.

### Caso A

Si es posible despejar $$x,y$$

$$
\left\{\begin{aligned}
&x=x(u,v) \\
&y=y(u,v)
\end{aligned}
\right. =
$$

Calculamos el Jacobiano de la transformación:

$$ J = \frac{\partial(x,y)}{\partial(u,v)} = 
\begin{array}{|cc|}
x'_{u} & x'_{v} \\
y'_{u} & y'_{v} \\
\end{array} \ne 0
$$

Luego,

$$\int\int_{R_{xy}} f(x,y)dx dy = \int\int_{R_{uv}} f[(x(u,v), y(u,v))] * |J| du dv $$

### Caso B

Puede suceder que no sea posible despejar $$x,y$$ en función de $$u,v$$

Entonces, calculamos directamente el jacobiano como:

$$ J =  \begin{array}{|cc|}
u'_{x} & u'_{y} \\
v'_{x} & v'_{y} \\
\end{array} \ne 0 
$$

Luego,

$$ \int\int_{R_{xy}} f(x,y) dx dy = \int\int_{R_{uv}} f(u,v)*\frac{1}{|J|} du dv $$

Podemos utilizar el caso B cuando también se puede hacer el despeje de $$x,y$$, según las cuentas puede resultar mas conveniente el cálculo por un caso o por el otro.

## Cambio a coordenadas polares

Supongamos que queremos integrar $$f(x,y)$$ sobre la región $$R: (x,y) \in \Re^2 / x^2+y^2 \le r_{0}$$, luego resulta mucho más conveniente para el cálculo de la integral, expresar $$R$$ con coordenadas polares.

$$
\left\{\begin{aligned}
&x=rcos(\theta) \\
&y=rsin(\theta)
\end{aligned}
\right. 0 \le r \le r_{0}; 0 \le \theta \le 2\pi
$$

luego, resolvemos por caso A

$$ J =  \begin{array}{|cc|}
x'_{r} & x'_{\theta} \\
y'_{r} & y'_{\theta} \\
\end{array} = r
$$

Ahora:

$$ \int\int_{R_{xy}} f(x,y) dx dy = \int_{0}^{r_{o}} \int_{0}^{2\pi} f(rcos(\theta), rsen(\theta)) * |r| d \theta dr $$

De la misma forma, si la región es una elipse:

$$R: (x,y) \in \Re^2 / \frac{x^2}{a^2}+\frac{y^2}{b^2} \le r_{0}$$

$$
\left\{\begin{aligned}
&x=arcos(\theta) \\
&y=brsin(\theta)
\end{aligned}
\right. 0 \le r \le r_{0}; 0 \le \theta \le 2\pi
$$

luego, resolvemos por caso A

$$ J =  \begin{array}{|cc|}
x'_{r} & x'_{\theta} \\
y'_{r} & y'_{\theta} \\
\end{array} = abr
$$

$$ \int\int_{R_{xy}} f(x,y) dx dy = \int_{0}^{r_{o}} \int_{0}^{2\pi} f(rcos(\theta), rsen(\theta)) * |abr| d \theta dr $$








