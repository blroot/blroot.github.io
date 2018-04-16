---
published: true
---
Límite,

## Límite

Sea la función $$ f:\Re^n \to \Re^m $$ ; $$ a \in \Re^m $$

y sea $$ \lim_{\vec x\to \vec a} f(\vec x) = \vec L $$

La definición formal de límite es muy similar a la de una variable

$$ \forall \epsilon > 0 \exists \delta > 0 : 0<dist(\vec x,\vec a)<\delta \implies 0<dist(f(\vec x), \vec L) $$

Es importante notar que SIEMPRE en límites de funciones multivariables, en todos los casos que tengamos una indeterminación de algún tipo y la "salvemos" hay que probar que el "potencial" límite existe!!

Ejemplo:

Calcular

$$ \lim_{(x,y)\to(a,a) = \frac{x^2-y^2}{x-y}} \\
= \lim_{(x,y)\to(a,a) = \frac{(x-y)(x+y)}{x-y}} = 2a $$

Hay que probar que el límite existe y es 2a por definición

$$ \forall \epsilon > 0 \exists \delta > 0 : 0<|| (x,y)-(a,a) ||<\delta \\
\implies abs(frac{x^2-y^2}{x-y}-2a) < \epsilon \\
abs(frac{(x-y)(x+y)}{x-y}-2a) < abs((x-a)+(y-a)) \leq |x-a|+|y-a| \\
\leq || (x-a;y-a) || + || (x-a;y-a) || \leq 2|| (x-a, y-a) || < 2 \delta
$$

Luego, encontramos una relación entre delta y épsilon

$$ \delta = \epsilon/2 $$

En conclusión, el límite existe y es $2a$