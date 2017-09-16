---
published: true
---
## Análisis matemático 1 - Topología

### Bola o entorno

Llamamos bola o entorno de centro $p$ y radio $r>0$ al conjunto:

$$ A={x\in R/|x-p|<r} = B(p,r) $$

Sea $A \in R$ se pueden clasificar los puntos de A de la siguiente manera:

### Punto interior

Sea $p \in R$ y $A \subseteq R$ un conjunto, se dice que "$p$ es interior a $A$"

$$ \iff \exists r>0 / B(p,r) \subset A $$

Por ejemplo:

Sea 

$$ A=[-2,3] \cup {7} $$

¿-1 es punto interior de A?

Luego, planteamos $p=-1$ y un $r>0$ por ejemplo $r=1$

$$ B(-1,1)=(-2,0) \subset A $$

$$ \implies $$ -1 es punto interior de A

¿7 es punto interior de A?

No, ya que $\nexists r>0 / B(7,r) \subset A$

En palabras, no se puede armar un entorno alrededor del 7

Se nota al conjunto de los puntos interiores de $A$ como $A^0$ 

En el ejemplo, $A^0=(-2,3)$

Se dice que un conjunto es abierto $\iff A=A^0$

En el ejemplo, $A \neq A^0 \implies A$ no es abierto 

### Punto clausura

Un punto $p$ es clausura de un conjunto $A \subseteq R$

$$ \iff \forall r>0 : B(p,r) \cap A \neq \varnothing $$

Con el mismo ejemplo: 

$$ A=[-2,3] \cup {7} $$

7 está en la clausura, 3 está en la clausura...

El conjunto de puntos clausura se nota $\overline{\rm A}$

$$ \overline{\rm A}=[-2,3] \cup 7 $$

Se dice que un conjunto es cerrado $\iff A=\overline{\rm A}$

### Punto frontera

Un punto $p \in R$ se dice frontera:

$$ \iff \forall r>0 : B(p,r) \cap A \neq \varnothing  \land B(p,r) \cap A^C \neq \varnothing$$

Donde $C$ es el complemento.

En el ejemplo, $aA={-2,3,7}$ es el conjunto de puntos frontera.



