---
published: true
---
límite, límites curvilineos, resolución por acotación, límites por coordenadas polares

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
\implies |\frac{x^2-y^2}{x-y}-2a| < \epsilon \\
|\frac{(x-y)(x+y)}{x-y}-2a| < |(x-a)+(y-a)| \leq |x-a|+|y-a| \\
\leq || (x-a;y-a) || + || (x-a;y-a) || \leq 2|| (x-a, y-a) || < 2 \delta
$$

Luego, encontramos una relación entre delta y épsilon

$$ \delta (\epsilon) = \frac{\epsilon}{2} $$

En conclusión, el límite existe y es $2a$

Otro ejemplo:

Demostrar que $$ \lim_{(x,y)\to(0,0)} \frac{4xy^2}{x^2+y^2} = 0 $$

Por definición:

$$ \forall \epsilon > 0 \exists \delta > 0 : 0 < || (x,y) - (0,0) ||< \delta \\
\implies 0<|\frac{4xy^2}{x^2+y^2}-0|<\epsilon 
$$

Tenemos que:

$$ 0<sqrt(x^2+y^2)<\delta \\
\implies |x|<\delta \land |y|<\delta
$$

Por propiedad, sabemos que $$ x^2+y^2 \ge y^2 $$
Luego:

$$ \frac{1}{x^2+y^2} \leq \frac{1}{y^2} $$

Multiplicando lado a lado por $$ 4|x|y^2 $$

$$ \frac{4|x|y^2}{x^2+y^2} \leq \frac{4|x|y^2}{y^2} \\
\leq 4|x|
$$

Como teníamos que $$ |x|<\delta $$

$$ \implies 4|x| < 4 \delta \implies \alpha (\epsilon) = \frac{\epsilon}{4} $$


