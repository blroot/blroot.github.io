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

1- $$ \int C*f(x)*dx=C \int f(x)*dx=C(P(x)+K)$$

2- $$ \int (f(x) \pm g(x))*dx=\int f(x)*dx \pm \int g(x)*dx \\ 
	  = P_{f}(x)+C_{1}+P_{g}(x)+C_{2} \\
      = P_{f}(x)+P_{g}(x)+C $$

3- $$ \int f'(x)*dx=f(x)+K $$

4- $$ (\int f(x)*dx)'=(P(x)+K)'=P'(x)=f(x) $$

La variable de integración importa!!

Por ejemplo:

$$ \int Sen(x)*dy = Sen(x)* \int 1*dy = Sen(x)*y+K $$

Como integramos con respecto a $y$, Sen(x) se trata como una constante.
Luego, como en una variable el concepto de derivada y diferencial son la misma cosa $\implies \int dy = y+K$

## Un ejemplo usando las propiedades y la tabla

$$ \int (2*Cos(x)+e^x+5*sqrt(x))*dx \\
   = \int 2*Cos(x)*dx + \int e^x*dx + \int 5*sqrt(x)*dx \\
   = 2* \int Cos(x)*dx + \int e^x*dx + 5* \int sqrt(x)*dx \\
   = 2*Sen(x)+e^x+5*2/3*x^(2/3) $$
   
### Métodos de resolución

Muchas veces vamos a tener integrales indefinidas que no pueden resolverse algebraicamente y/o por tabla

## Sustitución

En este método es clave saber que sustituír, en ningún caso deben quedar variables sin sustituír.

Ej: 

$\int x*e^(x^2)*dx$

Sustituímos $$x^2=t$$
aplicando diferencial de ambos lados 
$$x^2*dx=dt \\
  x*dx=dt/2 $$
  
Luego, $\int x*e^(x^2)*dx = \int e^t*dt/2 = 1/2* \int e^t*dt = 1/2*e^t+K$
Finalmente, sustituyendo nuevamente con la variable original $$ 1/2*e^(x^2)+K $$

## Partes

Cuando tengamos una integral de la forma $\int u*dv$
Podemos plantearla como $$ \int u*dv = u*v - \int v*du $$
Aquí tenemos que decidir que vamos a derivar y que vamos a integrar

Ej: $\int e^(3x)*Sen(x)*dx$

Por conveniencia, elijo derivar $e^(3x)$ e integrar $Sen(x)$

$$ u=e^(3x) \\
   du= 3*e^(3x)*dx $$

$$ dv=Sen(x)*dx \\
   v=-Cos(x) $$

$$ \implies \int e^(3x)*Sen(x)*dx = -e^(3x)*Cos(x)- \int -Cos(x)*3*e^(3x)*dx \\
   = -e^(3x)*Cos(x)+3* \int Cos(x)*e^(3x)*dx$$

*CA
Vuelvo a aplicar el método para $ \int Cos(x)*e^(3x)*dx $

$$ u=e^(3x) \\
   du= 3*e^(3x)*dx $$

$$ dv=Cos(x)*dx \\
   v=Sen(x) $$

$$ \int Cos(x)*e^(3x)*dx = e^(3x)*Sen(x)- \int Sen(x)*3*e^(3x)*dx \\
	= e^(3x)*Sen(x)-3* \int Sen(x)*e^(3x)*dx $$
    
Como podemos observar, $\int Sen(x)*e^(3x)*dx$ es la integral que originalmente queremos encontrar, entonces, vamos a resolver esta integral como una ecuación:

$$ \int Cos(x)*e^(3x)*dx = -e^(3x)*Cos(x)+3* [e^(3x)*Sen(x)-3* \int Sen(x)*e^(3x)*dx] \\
   = -e^(3x)*Cos(x)+3*e^(3x)*Sen(x)-9* \int Sen(x)*e^(3x)*dx \\
   = (-e^(3x)*Cos(x)+3*e^(3x)*Sen(x)/10) $$

## Fracciones simples

Dada una función racional $f(x)/g(x)$ se busca descomponer dicha función en una suma de fracciones de integración directa, $f(x)/g(x)$ debe ser irreductible!!

Ej: $\int x/(x^2-x-6)*dx$

Racionalizando.. $\int x/(x^2-x-6)*dx = \int x/((x-3)(x+2))*dx$

Aplicando el método, planteamos:

$$ x/((x-3)(x+2)) = A/(x-3) + B/(x+2) \\
   x = A(x+2)+B(x-3) $$

Resolviendo el sistema de ecuaciones, nos queda que
$B=2/5$ y $A=3/5$

Luego,

$$ \int x/(x^2-x-6)*dx = 3/5* \int 1/(x-3)*dx + 2/5* \int 1/(x+2)*dx $$

Aplicando el método de sustitución, nos va a quedar como:

$$ \int x/(x^2-x-6)*dx = 3/5*ln|x-3|+2/5*ln|x+2|+K $$




