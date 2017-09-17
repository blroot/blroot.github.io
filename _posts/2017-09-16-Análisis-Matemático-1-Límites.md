---
published: true
---
Límite de funciones en un punto, Álgebra de límites, Indeterminaciones, Teorema del sándwich, Continuidad.

## Límite de funciones

$$\lim_{x\to a} f(x) = L \in R \iff \forall \epsilon > 0, \exists \delta > 0 / \forall a \in Df : |x-a| < \delta \\ \implies |f(x)-L| < \epsilon$$

Por ejemplo:

$$\lim_{x\to 2} -3x+4 = -2$$ es candidato a límite

Sea $\epsilon = 0.1$ quiero hallar $ \delta > 0 / \lvert x-2 \lvert < \delta \implies \lvert f(x)+2 \lvert < 0,1 $

$$ \implies |f(x)+2|<0.1 \\ |-3x+4+2|<0.1 \\ |-3x+6|<0.1 \\ |-3(x-2)<0.1| \\ 3|x-2|<0.1 $$

Como queremos $ \lvert x-2 \lvert < \delta $

Decimos que:

$$ 3|x-2|<3\delta < 0.1 \\ 3\delta <0.1 \implies \delta < 0.1/3 $$

Generalizando:

Dado $\epsilon > 0$

$$ |f(x)+2|< \epsilon \\ |-3x+6|< \epsilon \\ 3|x-2|< \epsilon$$

De la definición de límite tenemos que $\lvert x-2 \lvert < \delta$

$$ \implies 3|x-2|<3\delta < 3\epsilon < \epsilon \\ 3\delta < \epsilon \\ \delta < \epsilon/3 $$

## Álgebra de límites

Sean $K$ constante, $f(x)$ y $g(x)$ dos funciones tales que:

$$ \lim_{x\to a} f(x) = L_{1}  $$ y $$ \lim_{x\to a} g(x) = L_{2}  $$

$$ \lim_{x\to a} f(x) + g(x) =  \lim_{x\to a} f(x) + \lim_{x\to a} g(x) = L_{1} + L_{2} $$

$$ \lim_{x\to a} K = K $$

$$ \lim_{x\to a} K * f(x) = K * \lim_{x\to a} f(x) = K.L_{1} $$

$$ \lim_{x\to a} f(x) * g(x) = \lim_{x\to a} f(x) * \lim_{x\to a} g(x) = L_{1} * L_{2} $$

$$ \lim_{x\to a} f(x) / g(x) = \lim_{x\to a} f(x) / \lim_{x\to a} g(x) = L_{1} / L_{2} $$

$$ (g o f)(x) \implies \lim_{x\to a} (g o f)(x) =  \lim_{x\to a} g(f(x)) \\ g(\lim_{x\to a} f(x)) = g(L_{1}) $$

En 11, $(g o f)(x)$ es continua.

## Indeterminaciones

$$ 0/0; \infty/\infty; \infty - \infty; 0* \infty; 1^\infty; \infty^0; 0^\infty $$

## Teorema del sándwich

Sean $f(x)$, $g(x)$, y $h(x)$ tres funciones tales que $f(x) \leq g(x) \leq h(x)$ y $\lim_{x\to a} f(x) = \lim_{x\to a} h(x) = L \in R \implies \lim_{x\to a} g(x) = L$

## Countinuidad en un punto

Sea $f(x)$ una función, se dice continua en un punto $a \iff \exists f(a) \land \lim_{x\to a^-} f(a) = \lim_{x\to a⁺} f(a) \land \lim_{x\to a} f(x) = f(a)$ 


