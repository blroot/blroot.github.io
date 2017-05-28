---
published: true
---
## Recordemos: Combinación Lineal

Decimos que un vector $\vec{v}$ puede escribirse como combinación lineal de los vectores del conjunto $A$ si se cumple que:

Sea $$A={\vec{\beta_{1}}, \vec{\beta_{2}},..., \vec{\beta_{n}}}$$

$$ \vec{v}=\alpha_{1}.\vec{\beta_{1}} + \alpha_{2}.\vec{\beta_{2}} +... \alpha_{n}.\vec{\beta_{n}} $$

Donde $$ \alpha_{1}, \alpha_{2}, \alpha_{n} \in R $$

Esto es más facil verlo en un ejemplo

Sean $$ \vec{v}=(2,1) $$
$$ A={(1,-1), (0,1)} $$

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

Se escribe $V=gen{\vec{1}, \vec{2}, \vec{n}}$

Es decir, el generador "genera" todo el espacio $V$, por lo tanto es una forma de expresar un espacio vectorial.

### Algunos ejemplos

$$ gen{(1,0),(0,1)}=R^2 $$
$$ gen{(1,0),(0,1),(1,1)}=R^2 $$
$$ gen{(1,0)}\notequalR^2 $$
$$ gen{(1,0,0),(0,1,0),(0,0,1)}=R^3 $$
