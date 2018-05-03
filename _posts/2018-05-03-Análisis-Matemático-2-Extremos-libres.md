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

Sea $$ f: \Re^2 \to \Re \wedge f''_{xx} \ne 0 \wedge f''_{xy} \ne 0 \wedge f''_{yx} \ne 0 \wedge f''_{yy} \ne 0 $$ tenemos la siguiente condición suficiente para la existencia de extremo:

$$
H = \begin{array}{|cc|}
f''_{xx} & f''_{xy} \\
f''_{yx} & f''_{yy} \\
\end{array}(x_{0}, y_{0})
$$

Entonces si:

$$ H>0  \implies $$ si $$f''_{xx}>0$$ mínimo en $$(x_{0}, y_{0}$$,
si $$f''_{xx}<0$$ máximo en $$(x_{0}, y_{0}$$

$$ H<0 \implies $$ punto de ensilladura en $$(x_{0}, y_{0}$$

$$ H=0 \implies $$ "casi extremo", si $$f''_{xx}>0$$ casi mínimo en $$(x_{0}, y_{0}$$, si $$f''_{xx}<0$$  casi máximo en $$(x_{0}, y_{0}$$

