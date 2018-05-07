---
published: true
---
Definición, forma cartesiana o implícita, curvas en $$\Re^3$$, clasificación de curvas, vector tangente o vector velocidad.

## Definición

Si pensamos en una curva de forma intuitiva como el trazo de un lápiz sobre una hoja, podemos decir que una parametrización de una curva, describe los puntos de la misma.
Vamos a llamar entonces curva a la gráfica de una función vectorial $$f:[t_{1},t_{2}] \to \Re^n / f(t)=(x_{1}(t), x_{2}(t)...x_{n}(t))$$

Por ejemplo:

$$ f:[0, 2*pi] \to \Re^2 / f(t)=(cos(t), sen(t)) $$

$$f(t)$$ es una parametrización de una circunferencia de radio 1 (llamémosla $$C$$), es importante notar que las parametrizaciónes de una curva no son únicas, por ejemplo, para la misma curva $$C$$, podemos tomar $$f:[0, 2*pi] \to \Re^2 / f(t)=(sen(t), cos(t))$$ que tiene trayectoria con sentido contrario a la primera.

## Forma cartesiana o implícita

El objetivo aquí es presentar la curva eliminando el parámetro $$t$$

$$
f(t) = \left\{\begin{aligned}
&x=cos(t) \\
&y=sen(t)
\end{aligned}
\right. =
$$
$$
\left\{\begin{aligned}
&x^2=cos^2(t) \\
&y^2=sen^2(t)
\end{aligned}
\right.
$$ 

$$\implies x^2+y^2=1$$ es una ecuación implícita de $$C$$

## Curvas en $$\Re^3$$

## Clasificación de curvas

Suponiendo una función que describe una curva de la forma $$C:[a,b] \to \Re^n$$ continua

### curva cerrada
Si $$C(a) = C(b) \implies$$ la curva es cerrada
Si $$C(a) \ne C(b) \implies$$ la curva es abierta

### curva simple
Una curva se dice simple, si la parametrización que la define es inyectiva, esto significa que la curva no posee autointersecciones.

Si alguna de las funciones coordenadas de la parametrización es inyectiva, es suficiente para decir que la parametrización también lo es, caso contrario, debemos recurrir a la definición de inyectividad:

$$C(t_{1})=C(t_{2}) \iff t_{1}=t_{2}$$

### curva regular
Una curva es regular si se cumple que $$||C'(t)|| \ne 0$$.
Gráficamente, si la curva no es regular en un punto, presenta un vértice o pliegue en el mismo.


