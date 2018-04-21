---
published: true
---
Derivadas parciales, vector gradiente, plano tangente, derivadas direccionales

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

De manera muy similar, la derivada en un punto $$ (x_{0}, y_{0}) $$:

$$ \frac{\partial f}{\partial x}(x_{0}, y_{0}) = f'_{x}(x_{0}, y_{0}) = \lim_{h \to o } \frac{f(x_{0}+h, y_{o})-f(x_{o},y_{0})}{h} $$

$$ \frac{\partial f}{\partial y}(x_{0}, y_{0}) = f'_{y}(x_{0}, y_{0}) = \lim_{h \to o } \frac{f(x_{0}, y_{0}+h)-f(x_{0},y_{0})}{h} $$
