---
published: true
---
Derivadas parciales, derivabilidad y continuidad, vector gradiente, plano tangente, derivadas direccionales, maximización de la derivada direccional, derivadas de $$ R^n $$

## Derivadas parciales

Si venimos del análisis de una variable, para derivar una función de dos o mas variables, se nos presenta el siguiente problema: ¿A partir de que variable derivamos?
Las derivadas en dos o mas variables son direccionales, es decir se calculan a través de algún vector.
En una funcion $$ f:\Re^2 \to \Re $$ Las derivadas parciales, son aquellas derivadas calculadas a partir de los versores $$ \hat{x} $$ e $$ \hat{y} $$ 

Entonces:

$$ f:\Re^2 \to \Re / f(x,y)=z $$

sus derivadas parciales se notan como

$$ \frac{\partial f}{\partial x} $$ o también $$ f'_{x} $$

$$ \frac{\partial f}{\partial y} $$ o también $$ f'_{y} $$

Para calcular las derivadas parciales (genéricas), de manera similar a una variable, tenemos el límite del cociente incremental:

$$ \frac{\partial f}{\partial x} = f'_{x} = \lim_{h \to o } \frac{f(x+h, y)-f(x,y)}{h} $$

$$ \frac{\partial f}{\partial y} = f'_{y} = \lim_{h \to o } \frac{f(x, y+h)-f(x,y)}{h} $$

De manera muy similar, las derivadas parciales en un punto $$ (x_{0}, y_{0}) $$:

$$ \frac{\partial f}{\partial x}(x_{0}, y_{0}) = f'_{x}(x_{0}, y_{0}) = \lim_{h \to o } \frac{f(x_{0}+h, y_{o})-f(x_{o},y_{0})}{h} $$

$$ \frac{\partial f}{\partial y}(x_{0}, y_{0}) = f'_{y}(x_{0}, y_{0}) = \lim_{h \to o } \frac{f(x_{0}, y_{0}+h)-f(x_{0},y_{0})}{h} $$

Ej: Hallar las derivadas parciales de la función $$ f(x,y)=x^2+3y $$ en $$ P_{0}=(2,-1) $$

$$ f'_{x}(2,-1) = \lim_{h \to 0} \frac{f(2+h, -1)-f(2,-1)}{h} \\
\lim_{h \to 0} \frac{(2+h)^2+3(-1)-1}{h} = \lim_{h \to 0} \frac{h(4+h)}{h} = 4
$$

$$ f'_{y}(2,-1) = \lim_{h \to 0} \frac{f(2, -1+h)-f(2,-1)}{h} \\
\lim_{h \to 0} \frac{4+(-3+3h)-1}{h} = \lim_{h \to 0} \frac{3h}{h} = 3
$$

También podemos hacerlo por el método que conocemos de análisis en una variable

$$ f'_{x} = 2x; f'_{x}(2,-1)=4 $$

$$ f'_{y} = 3; f'_{y}(2,-1)=3 $$

Cuidado porque esto en ocasiones no funciona cuando la derivada presenta discontinuidades:
Ej: Calcular derivada parcial en x de  $$ f(x,y)=\sqrt[3]{x^3+y^3} $$ en $$ (0,0) $$

Por definición:

$$ f'_{x}(0,0) = \lim_{h \to 0} \frac{f(0+h,0)-f(0,0)}{h} = \lim_{h \to 0} \frac{\sqrt[3]{h^3}}{h} = 1 $$

Por método "directo":

$$ f'_{x} = \frac{x^2}{\sqrt[3]{(x^3+y^3})^2} \implies f'_{x}(0,0)= \frac{0}{0} $$

Como podemos ver, nos queda una indeterminación, por lo que en esos casos debemos recurrir a la definición.

## Derivabilidad y continuidad

Sea:

$$
f(x,y) = \left\{\begin{aligned}
&\frac{xy}{x^2+y^2} &&: (x,y) \neq (0,0) \\
&0 &&: (x,y) = (0,0)
\end{aligned}
\right.$$

1- Hallar derivabilidad en $$(0,0)$$
2- Hallar si existen las derivadas parciales en $$(0,0)$$

1- Tenemos que $$ \frac{xy}{x^2+y^2} $$ es continua $$ \forall (x,y) \neq (0,0) $$ por ser un cociente de polinomios.

Analizamos entonces que sucede en $$(0,0)$$

Por familia de rectas:

$$ \lim_{(x,y) \to (0,0);y=mx} \frac{xy}{x^2+y^2} = \lim_{x \to 0} \frac{mx^2}{x^2(1+m^2)} = \frac{m}{1+m^2} \implies \nexists \lim  \implies f $$ no es continua en $$ (0,0) $$

2- Como existe imágen de f en (0,0) y vale 0, pueden existir las derivadas parciales:

$$ f'_{x}(0,0) = \lim_{h \to 0} \frac{f(0+h,0)-f(0,0)}{h} = \lim_{h \to 0} \frac{h*0}{\frac{h^2+0^2}{h}} = 0 $$

$$ f'_{y}(0,0) = \lim_{h \to 0} \frac{f(0,0+h)-f(0,0)}{h} = \lim_{h \to 0} \frac{0*h}{\frac{0^2+h^2}{h}} = 0 $$

Como podemos ver, en dos o más variables, la derivabilidad no guarda relación con la continuidad, el único requisito para que las derivadas parciales existan, es exista la imágen de la función en el punto en el cual calcular las derivadas parciales.

## Vector gradiente

Las derivadas parciales en un punto de una función $$f$$, definen un vector llamado gradiente y se nota como: $$ \vec{\nabla f} $$

$$ \vec{\nabla f} = (\frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}) $$

## Plano tangente

Las derivadas parciales, definen un plano tangente que se obtiene de la siguiente forma:

Sea $$ f: \Re^2 \to \Re $$ el plano tangente en $$ (a,b) $$

$$ z = f(a,b) + \frac{\partial f}{\partial x}(x-a) + \frac{\partial f}{\partial y}(y-b) $$

o de forma equivalente:

$$ z = f(a,b) + \vec{\nabla f(a,b)} * (x-a, y-b) $$

Cuando veamos diferenciabilidad, vamos a ver que llamar a este plano "tangente" es en realidad un abuso de lenguaje, ya que no siempre se cumple que el plano satisfaga la condición  de tangencia.

Ej:

Calcular el plano tangente a la función $$ f(x,y) = x^2+y^4+e^{xy}+7 $$ en $$P_{0}=(1,0,9)$$

Calculo derivadas parciales en $$ (1,0) $$:

$$ f'_{x} = 2x+ye^{xy} \implies f'_{x}(1,0) = 2 $$

$$ f'_{y} = 4y^3+xe^{xy} \implies f'_{y}(1,0) = 1 $$

Luego el plano queda como:

$$ z = f(1,0) + 2(x-1) + 1(y-0) \\
= 9 + 2(x-1) + y \implies pi: 2x+y-z+7=0
$$

## Derivadas direccionales

Como mencionamos en la primera parte, las derivadas parciales son calculadas a partír de una dirección, es decir, un versor correspondiente al eje de la base sobre el cual queremos derivar.
Entonces, la derivada a partir de un vector versor $$ \vec{v} = (a,b) $$ se calcula como:

$$ f'_{\vec{v}(x_{o}, y_{o})} = \lim_{t \to 0} \frac{f[(x_{0},y_{0}+t(a,b))]-f(x_{0},y_{0})}{t} \\
= \lim_{t \to 0} \frac{f(x_{0}+ta, y_{0}+tb)-f(x_{0}, y_{0})}{t}
$$

Si calculamos la derivada respecto a $$ \vec{w} = (1,0) $$ (versor x) vamos a obtener la derivada respecto de x. Por otro lado, si calculamos la derivada respecto a $$ \vec{z} = (0,1) $$ (versor y) vamos a obtener la derivada respecto de y.

## Maximización de la derivada direccional

El valor máximo de la derivada direccional 
$$D_{\vec u} f(x)$$ 
es 
$$|\nabla f(x)|$$ y se presenta cuando $$\vec u$$ tiene la misma dirección que el vector gradiente.

## Derivadas de $$ R^n $$

Sea $$ f:\Re^n \to \Re^m $$. Las derivadas de estas funciones se presentan con una matriz jacobiana

$$ J = \begin{bmatrix}
              f'_{1_{x1}} & f'_{1_{x2}} & f'_{1_{x3}} \\
              f'_{2_{x1}} & f'_{2_{x2}} & f'_{2_{x3}} \\
              f'_{3_{x1}} & f'_{3_{x2}} & f'_{3_{x3}}
\end{bmatrix} $$

Ej: Hallar la derivada de $$ f(x,y,z) $$ en $$P_{0}=(1,2,0)$$

$$ f(x,y,z)=(x^2+3y^2-8z, 5x^2y^3e^z) $$

Como es una función de $$\Re^3 \to \Re^2 \implies J \in \Re^{2x3}$$

$$ 
J = \begin{bmatrix}
              f'_{1x} & f'_{1y} & f'_{1z} \\
              f'_{2x} & f'_{2y} & f'_{2z}
\end{bmatrix} =

\begin{bmatrix}
              2x & 6y & -8 \\
              10xy^3e^z & 15x^2y^2e^z & 5x^2y^3e^z
\end{bmatrix} =

\begin{bmatrix}
              2 & 12 & -8 \\
              80 & 60 & 40
\end{bmatrix} 
$$
