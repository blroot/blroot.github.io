---
published: true
---
Derviadas sucesivas o de órden superior, teorema de Schwarz, aproximación cuadrática (polinomio de Taylor de grado 2)

## Derivadas sucesivas o de órden superior

Como ya vimos, en funciones de varias variables derivamos parcialmente, en las derivadas sucesivas también sucede lo mismo, Sea $$f: \Re^2 \to \Re$$ podemos derivar $$f$$ respecto de $$x$$ ($$f'_{x}$$)
y luego con respecto a $$y$$ ($$f''_{xy}$$).

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

Ejercicio:

Averiguar el mínimo $$n \in N / D_{x}D_{y}f(0,0)=D_{y}D_{x}f(0,0)$$

sea 
$$
f(x,y) = \left\{\begin{aligned}
&\frac{x^ny}{x^2+y^2} &&: (x,y) \neq (0,0) \\
&0 &&: (x,y) = (0,0)
\end{aligned}
\right.$$

Analizando continuidad:

$$ \lim_{(x,y) \to (0,0)} \frac{x^ny}{x^2+y^2} = 0 $$

Acotando 

$$ x^2+y^2 \ge y^2 $$

$$ \frac{1}{x^2+y^2} \le \frac{1}{y^2} $$

luego

$$ \frac{|x^n||y|}{x^2+y^2} \le \frac{|x^n||y|}{y^2} \le |x^n| $$

Por sandwich, $$ \lim_{(x,y) \to (0,0)} \frac{x^ny}{x^2+y^2} = 0 $$
entonces es continua en $$(0,0)$$

Obtengo las derivadas parciales:

Si $$(x,y) \neq (0,0)$$

$$ f'_{x} = \frac{y(nx^{n-1}(x^2+y^2)-2x^{n+1})}{(x^2+y^2)^2} $$
$$ f'_{y} = \frac{x^n(x^2+y^2-2y^2)}{(x^2+y^2)^2} $$

Si $$(x,y) = (0,0)$$

$$ f'_{x} = 0 $$
$$ f'_{y} = 0 $$

Y ahora las derivadas cruzadas en $$(0,0)$$

$$ f''_{yx} = \lim_{h \to 0} \frac{f'_{y}(h,0)-f'_{y}(0,0)}{h} = \lim_{h \to 0} \frac{h^n}{h^3} $$

$$ f''_{xy} = \lim_{h \to 0} \frac{f'_{x}(0,h)-f'_{x}(0,0)}{h} = 0 $$

Como los límites deben coincidir, igualo:

$$ \lim_{h \to 0} \frac{h^n}{h^3} = 0  \iff n \ge 4 $$

En conclusión, el mínimo $$n \in N / D_{x}D_{y}f(0,0)=D_{y}D_{x}f(0,0)$$ es $$4$$

## Aproximación cuadrática

Como ya vimos, la aproximación lineal de una función de dos variables se calcula mediante el plano tangente en un punto $$(a,b)$$

$$T(x,y)=f(a,b)+f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b)$$

Lo anterior se denomina también polinomio de Taylor de primer grado de $$f$$ en $$(a,b)$$

De la misma manera, definimos el polinomio de Taylor de grado 2 de una función $$f$$ de dos variables en $$(a,b)$$ como:

$$Q(x,y)=f(a,b)+f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b) \\ + \frac{1}{2}f_{xx}(a,b)(x-a)^2+f_{xy}(a,b)(x-a)(y-b)+\frac{1}{2}f_{yy}(a,b)(y-b)^2$$