---
published: true
---
## Recordemos: Combinación Lineal

Decimos que un vector $\vec{v}$ puede escribirse como combinación lineal de los vectores del conjunto $A$ si se cumple que:

Sea $$A={\vec{\beta_{1}}, \vec{\beta_{2}},..., \vec{\beta_{n}}}$$

$$ \vec{v}=\alpha_{1}.\vec{\beta_{1}} + \alpha_{2}.\vec{\beta_{2}} +... \alpha_{n}.\vec{\beta_{n}} $$

Donde $$ \alpha_{1}, \alpha_{2}, \alpha_{n} \in R $$

Esto es más facil verlo en un ejemplo

Sean $$ \vec{v}=(2,1); $$
$$ A=\{(1,-1), (0,1)\} $$

Entonces ¿Es $\vec{v}$ combinación lineal de $(1,-1)$ y $(0,1)$?  
Para ver esto, planteamos:

$$ \alpha_{1}(1,-1) + \alpha_{2}(0,1)=(2,1) $$
$$ (\alpha_{1}, -\alpha_{1}) + (0, \alpha_{2})=(2,1) $$
$$ (\alpha_{1}, -\alpha_{1}+\alpha_{2})=(2,1) $$

Si observamos bien, podemos plantear un sistema de ecuaciones lineales

$$ \begin{cases} \alpha_{1}=2 \\ -\alpha_{1}+\alpha_{2}=1 \end{cases} $$

$$ => \alpha_{1}=2 \hspace{0.5cm} \alpha_{2}=3 $$

Tenemos que $$(2,1)=2(1,-1)+3(0,1)$$  
Entonces decimos que $\vec{v}$ es combinación lineal de $(1,-1)$ y $(0,1)$

## Sistema generador

Un conjunto de vectores es un sistema generador de un $K$-espacio vectorial $V$ si cualquier vector de $V$ puede escribirse como combinación lineal de los vectores del sistema generador.

Se escribe $$ gen\{\vec{v_1}, \vec{v_2},..., \vec{v_n}\}$$

Es decir, el generador "genera" todo el espacio $V$, por lo tanto es una forma de expresar un espacio vectorial.

### Algunos ejemplos

$$ gen\{(1,0),(0,1)\}=R^2$$  
$$ gen\{(1,0),(0,1),(1,1)\}=R^2 $$  
$$ gen\{(1,0)\} \neq R^2 $$  
$$ gen\{(1,0,0),(0,1,0),(0,0,1)\}=R^3 $$  

## Independecia lineal y Dependencia lineal

Se dice que un conjunto es linealmente independiente cuando el vector nulo es combinación lineal de los vectores de dicho conjunto solo con los coeficientes iguales a cero. Veámoslo formalmente:

Sea $V$ un $K$-espacio vectorial y un conjunto $$A=\{\vec{v_1}, \vec{v_2}, \vec{v_n}\} \in V$$  
decimos que $A$ es linealmente independiente si:  

$$ \vec{v}=\alpha_{1}.\vec{v_{1}} + \alpha_{2}.\vec{v_{2}} +... \alpha_{n}.\vec{v_{n}}=\vec{0} $$  
Con $\alpha_{i}=0$ para todo $i$

Por otro lado es linealmente dependiente si el vector nulo es combinación lineal de los vectores del conjunto con alguno o algunos de los coeficientes distinto o distintos de cero.

Sea $V$ un $K$-espacio vectorial y un conjunto $$A=\{\vec{v_1}, \vec{v_2}, \vec{v_n}\} \in V$$  

decimos que $A$ es linealmente dependiente si: 

$$ \vec{v}=\alpha_{1}.\vec{v_{1}} + \alpha_{2}.\vec{v_{2}} +... \alpha_{n}.\vec{v_{n}}=\vec{0} $$  
Con $\alpha_{i} \neq 0$ para algún $i$

Vamos a ver ejemplos de esto en bases de un espacio vectorial

## Base de un espacio vectorial

Sea $V$ un $K$-espacio vectorial, decimos que un conjunto $$A=\{\vec{v_1}, \vec{v_2}, \vec{v_n}\}$$ es una base de $V$ si cumple que:

- $A$ es linealmente independiente
- $gen\{A}\}=V$

De los ejemplos de generadores, vimos que $$ gen\{(1,0),(0,1)\}=R^2 $$

Tenemos que $\{(1,0),(0,1)}\}$ genera $R^2$ pero ¿Es linealmente independiente?  
Para eso planteamos:  

$$  \alpha_{1}(1,0) + \alpha_{2}(0,1)=(0,0) $$  
$$ (\alpha_{1}, 0) + (0, \alpha_{2})=(0,0) $$  
$$ (\alpha_{1}, \alpha_{2})=(0,0) $$

Nos queda que $\alpha_{1}=0$ y $\alpha_{2}=0$, por lo tanto el conjunto es linealmente independiente.  
Entonces $B=\{(1,0),(0,1)}\}$ es una base de $R^2$  

### Dimensión de una base

La dimensión de una base, es basicamente la cantidad de vectores que contiene dicha base.
En el ejemplo anterior vimos que $B=\{(1,0),(0,1)}\}$ es una base de $R^2$  
Por lo tanto la dimensión de $B$ es igual a $2$  
Se escribe:  

$$ Dim(B)=2 $$

Nótese que la dimensión de una base de $R^2$ siempre tiene dimensión $2$ y una base de $R^3$ siempre va a tener dimensión $3$

**Observación**: 

A \{(1,0),(0,1)}\} se la conoce como base canónica de $R^2$

¿Te suena la notación de vectores en R^2 y R^3 respectivamente como $v=\alpha i+\beta j$ y $v=\alpha i+\beta j+\gamma k$?

Esta notación es la combinación lineal de un vector a partir de la base canónica, geométricamente $i$, $j$ y $k$ son los versores de cada eje  

En $R^3$  
$$ (x, y, z) =  \alpha i + \beta j$ + \gamma k$$  
Es lo mismo que  
$$ (x, y, z) =  \alpha (1,0,0) + \beta (0,1,0)$ + \gamma (0,0,1) $$  


Bien, ahora ¿Qué sucede si tenemos un conjunto que genera un espacio vectorial pero no es linealmente independiente? ¿Cómo obtenemos una base en ese caso?

De los ejemplos de generadores, vimos que $$ gen\{(1,0),(0,1),(1,1)\}=R^2 $$  
Bien, \{(1,0),(0,1),(1,1)\} genera $R^2$ pero ¿Es linealmente independiente? Para eso planteamos: 

$$  \alpha_{1}(1,0) + \alpha_{2}(0,1) + \alpha_{3}(1,1)=(0,0) $$  

El sistema queda

$$ \begin{cases} \alpha_{1}+\alpha_{3}=0 \\ \alpha_{2}+\alpha_{3}=0 \end{cases} $$












