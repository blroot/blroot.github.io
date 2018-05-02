---
published: true
---
Derviadas sucesivas o de órden superior, teorema de Schwarz

## Derivadas sucesivas o de órden superior

Como ya vimos, en funciones de varias variables derivamos parcialmente, en las derivadas sucesivas también sucede lo mismo, Sea $$f: \Re^2 \to \Re$$ podemos derivar $$f$$ respecto de $$x$$ ($$f'_{x}$$)
y luego con respecto a $$y$$ ($$f'_{xy}$$).

Ej:

Sea $$ f(x,y)=xy+(x+2y)^2 $$

Las derivadas de primer órden son:

$$f'_{x}=y+2(x+2y)$$; $$f'_{y}=x+4(x+2y)$$

las de segundo órden:

$$f''_{xx}=2$$; $$f''_{yy}=8$$

y de segundo órden mixtas:

$$f''_{xy}=5$$; $$f''_{yx}=5$$

Nótese que las derivadas de segundo órden mixtas en este caso son iguales. esto no es casualidad.

## Teorema de Schwarz

Si $$D_{1}f(x,y)$$ y $$D_{2}f(x,y)$$ son diferenciables en un entorno de $$a \implies D_{1}f(a)=D_{2}f(a)$$

En palabras, si se cumple que las derivadas de primer orden son diferenciables en $$a$$, entonces las derivadas mixtas en cualquier órden de derivación de segundo órden son iguales.
Esto se puede generalizar para órdenes mayores:

Las derivadas mixtas de órden $$n$$ en $$a$$ van a ser iguales $$\iff$$ las derivadas de órden $$n-1$$ son diferenciables en $$a$$
