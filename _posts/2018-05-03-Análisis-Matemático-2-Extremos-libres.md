---
published: true
---
Mínimo, máximo, punto de ensilladura, condición necesaria para existencia de extremo, cálculo de hessiano, condición suficiente para existencia de extremo.

## Mínimo, máximo, punto de ensilladura

Decimos que una función presenta un **mínimo** en $$(x_{0}, y_{0})$$ si $$\forall (x,y)$$ perteneciente al entorno del mismo se cumple que 

$$ \Delta Z = f(x,y)-f(x_{0}, y_{0})>0 $$

Decimos que una función presenta un **máximo** en $$(x_{0}, y_{0})$$ si $$\forall (x,y)$$ perteneciente al entorno del mismo se cumple que 

$$ \Delta Z = f(x,y)-f(x_{0}, y_{0})<0 $$

Decimos que $$f(x,y)$$ presenta **punto de silla** en un punto $$(x_{0}, y_{0})$$ si para ciertos valores $$(x,y)$$ de dicho entorno se cumple $$ \Delta Z = f(x,y)-f(x_{0}, y_{0})>0 $$ para algunos valores y $$ \Delta Z = f(x,y)-f(x_{0}, y_{0})<0 $$ para otros valores.

## Condición necesaria para existencia de extremo

La condición necesaria (no suficiente) en un punto $$ (x_{0}, y_{0}) $$ de $$ Z=f(x,y) $$ es que las derivadas parciales existan en dicho punto y sean iguales a cero.

## Cálculo de hessiano

Sea $$ f: \Re^2 \to \Re  $$ y al menos una de las derivadas segundas de $$f$$ en $$(x_{0}, y_{0})$$ distintas de cero, tenemos la siguiente condición suficiente para la existencia de extremo en $$(x_{0}, y_{0})$$:

$$
H = \begin{array}{|cc|}
f''_{xx} & f''_{xy} \\
f''_{yx} & f''_{yy} \\
\end{array}(x_{0}, y_{0})
$$

Entonces si:

$$ H>0  \implies $$ si $$f''_{xx}>0 \implies $$ mínimo en $$(x_{0}, y_{0})$$,
si $$f''_{xx}<0 \implies $$ máximo en $$(x_{0}, y_{0})$$

$$ H<0 \implies $$ punto de ensilladura en $$(x_{0}, y_{0})$$

$$ H=0 \implies $$ "casi extremo", si $$f''_{xx}>0 \implies $$ casi mínimo en $$(x_{0}, y_{0})$$, si $$f''_{xx}<0 \implies $$  casi máximo en $$(x_{0}, y_{0})$$

## Condición suficiente para existencia de extremo

Como vimos, no podemos utilizar el hessiano cuando todos sus coeficientes son nulos. Podemos utilizar lo que vimos en la definición para demostrar la existencia de un extremo:

Ej:

Hallar los extremos de $$f(x,y)=(x-y)^4+(y-1)^4$$

Busco los puntos críticos:

$$f'_{x}=4(x-y)^3=0 \iff x=y$$

$$f'_{y}=-4(x-y)^3+4(y-1)^3=0 \iff x=y \wedge y=1$$

$$ \implies P_{0}=(1,1)$$

Hallo las derivadas cruzadas:

$$f''_{xx}=12(x-y)^2 ; f''_{yy}=12(x-y)^2+12(y-1)^2$$

$$f''_{xy}=-12(x-y)^2 $$

Como vemos, en este caso todas las derivadas segundas nos dan $$0$$ en $$(P_{0})$$ entonces el hessiano no decide.

Por definición:

$$ f(x,y)-f(1,1) = (x-y)^4+(y-1)^4-0 $$

Como podemos ver, nos queda una suma de dos cosas positivas, entonces:

$$ (x-y)^4+(y-1)^4 > 0 \implies P_{0}$$ es mínimo absoluto, porque esto se cumple $$ \forall (x,y) \ne (1,1) $$ 




