---
published: true
---
Límite de funciones en un punto, Álgebra de límites, Indeterminaciones, Teorema del sandwich.

## Límite de funciones

$$\lim_{x\to a} f(x) = L \in R \iff \forall \epsilon > 0, \exists \delta > 0 / \forall a \in Df : |x-a| < \delta \implies |f(x)-L| < \epsilon$$

Por ejemplo:

$$ \lim_{x\to 2} -3x+4 = -2 $$ es candidato a límite

Sea $\epsilon = 0.1$ quiero hallar $\delta > 0 / |x-2|< \delta \implies |f(x)+2|< 0,1$

$$ \implies |f(x)+2|<0.1 \newline |-3x+4+2|<0.1 \newline |-3x+6|<0.1 \newline |-3(x-2)<0.1| \newline 3|x-2|<0.1 $$

Como queremos $|x-2|< \delta$

Decimos que:

$$ 3|x-2|<3\delta < 0.1 \newline 3\delta <0.1 \implies \delta < 0.1/3 $$

Generalizando:

Dado $\epsilon > 0$

$$ |f(x)+2|< \epsilon \newline |-3x+6|< \epsilon \newline 3|x-2|< \epsilon$$

De la definición de límite tenemos que $|x-2|< \delta$

$$ \implies 3|x-2|<3\delta < 3\epsilon < \epsilon \newline 3\delta < \epsilon \newline \delta < \epsilon/3 $$

