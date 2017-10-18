---
published: true
---
Primitiva, Una tabla de integrales, Propiedades, Métodos de integración

## Integral indefinida

Decimos que $P(x)$ es primitiva de $f(x) \iff P'(x)=f(x)$

Ej: Sea $f(x)=2$
Una primitiva de $f(x)$ es $P(x)=2x$, pero esta no es única, ya que por ejemplo, $Q(x)=2x+1$ también es primitiva de $f(x)$

Luego, a partir de cualquier función $f(x)$ existe una familia de infinitas primitivas, que difieren entre sí solo en su constante.

Llamaremos integral indefinida al conjunto de todas las primitivas que admite una función $f(x)$ la cual notaremos:

$$ \int f(x) * dx = P(x)+K $$

Donde "Sigma" indica que se trata de una integral indefinida.
$dx$ "Diferencial x" indica la variable de integración.
$K \in R$.

## Algunas integrales

$$ \int C*dx = Cx+K $$
$$ \int x^n*dx = x^(n+1)/(n+1) $$
$$ \int 1/x*dx = ln|x|+K $$
$$ \int e^x*dx = e^x+K $$
$$ \int Sen(x)*dx = -Cos(x)+K $$
$$ \int Cos(x)*dx = Sen(x)+K $$
$$ \int 1/(1+x^2)*dx = arctg(x)+K $$
$$ \int 1/sqrt(1-x^2)*dx = arcsen(x)+K $$

## Propiedades

Sean $f$ y $g$ dos funciones definidas en un dominio común

1- $$ \int C*f(x)*dx=C \int f(x)*dx=C(P(x)+K) ; C \in R $$

2- $$ \int (f(x) \pm g(x))*dx=\int f(x)*dx \pm \int g(x)*dx \\ 
	  = P_{f}(x)+C_{1}+P_{g}(x)+C_{2} \\
      = P_{f}(x)+P_{g}(x)+C $$

3- $$ \int f'(x)*dx=f(x)+K $$

4- $$ (\int f(x)*dx)'=(P(x)+K)'=P'(x)=f(x) $$

La variable de integración importa!!

Por ejemplo:

$$ \int Sen(x)*dy = Sen(x)* \int 1*dy = Sen(x)*y+K $$

Como integramos con respecto a $y$, Sen(x) se trata como una constante.
Luego como en una variable el concepto de derivada y diferencial son la misma cosa $\implies \int dy = y+K$

## Un ejemplo usando las propiedades y la tabla

$$ \int (2*Cos(x)+e^x+5*sqrt(x))*dx \\
   = \int 2*Cos(x)*dx + \int e^x*dx + \int 5*sqrt(x)*dx \\
   = 2* \int Cos(x)*dx + \int e^x*dx + 5* \int sqrt(x)*dx \\
   = 2*Sen(x)+e^x+5*2/3*x^(2/3) $$
   

