---
published: true
---
Contacto de orden n entre dos funciones, test de tangencia, teoremas.

## Contacto de orden n entre dos funciones

Dos funciones $$ f $$ y $$ g $$ tienen un contacto de orden $$ n $$ en el punto $$ a  $$ cuando:

$$ \lim_{x \to a} \frac{f(x)-g(x)}{|| x-a ||^n} = 0 $$

## Test de tangencia

Cuando hablamos de tangencia, estamos hablando de un contacto de orden 1 entre dos funciones.

Luego, sea $$ f:\Re^2 \to \Re $$ entonces la función posiblemente tangente en $$ (a,b) $$ será de la forma $$ Z=f(x,y) $$

$$ \implies Z=T(x,y)= f(a,b) + \frac{\partial f}{\partial x}(x-a) + \frac{\partial f}{\partial y}(y-b) $$

Es el plano "tangente" que vimos durante derivabilidad. Vamos ahora a llamar a este plano, posiblemente o potencialmente tangente, para verificar que efectivamente el plano es tangente, debemos hacer la prueba de tangencia:

$$ \lim_{(x,y) \to (a,b)} \frac{f(x,y)-T(x,y)}{|| x-a, y-b ||}=0 $$

Finalmente, si el plano es tangente en $$ (a,b) $$ decimos que $$ f $$ es diferenciable en $$ (a,b) $$

## Teoremas

1* Si $$ \frac{\partial f}{\partial x}(x,y) $$ y $$ \frac{\partial f}{\partial y}(x,y) $$ son continuas en un entorno de $$ (a,b) \implies $$ $$ f $$ es diferenciable en $$ (a,b) $$

2* Si $$ f $$ es diferenciable en $$ (a,b) \implies$$ $$ f $$ es continua en $$ (a,b) $$
