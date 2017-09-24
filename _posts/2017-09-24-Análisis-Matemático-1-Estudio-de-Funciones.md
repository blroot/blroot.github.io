---
published: true
---
Teoremas de derivación en intervalos cerrados (Rolle, Fermat), Extremos, Crecimiento y decrecimiento, Mínimos y máximos, Teorema de Lagrange, Concavidad y convexidad.

## Teorema de Rolle

Sea $f:[a,b]->R$ continua y derivable en $(a,b)$ y tal que $f(a)=f(b)$ luego $\exists c \in (a,b) / f'(c)=0$

## Teorema de Fermat

Sea $f:[a,b]->R$ derivable en un punto $x=c$ y tal que presenta un extremo relativo en $x=c \implies f'(c)=0$

## Extremos de una función

Sea $f:D \subseteq R -> R$ una función, diremos que $f$ presenta un **máximo relativo** en $x=a \iff \exists \delta > 0 / \forall x \in (a- \delta; a+ \delta) : f(a) \geq f(x)$

Sea $f:D \subseteq R -> R$ una función, diremos que $f$ presenta un **mínimo relativo** en $x=b \iff \exists \delta > 0 / \forall x \in (b- \delta; b+ \delta) : f(b) \leq f(x)$

Sea $f:D \subseteq R -> R$ una función, diremos que $f$ presenta un **máximo absoluto** en $x=c \iff : f(c) \geq f(x) \forall x \in Df$

Sea $f:D \subseteq R -> R$ una función, diremos que $f$ presenta un **mínimo absoluto** en $x=c \iff : f(c) \leq f(x) \forall x \in Df$

## Teorema de Lagrange

Sea $f$ una función continua en $[a,b]$ y derivable en $(a,b)$. Entonces $\exists c \in (a,b) / f'(c)=(f(b)-f(a))/(b-a)$

### Consecuencias de teorema de Lagrange

Si $f' \geq 0$ en $(a,b) \implies f$ es **creciente** en $(a,b)$
Si $f' > 0$ en $(a,b) \implies f$ es **estrictamente creciente** en $(a,b)$

Si $f' \leq 0$ en $(a,b) \implies f$ es **decreciente** en $(a,b)$
Si $f' < 0$ en $(a,b) \implies f$ es **estrictamente decreciente** en $(a,b)$

## Concavidad y convexidad de una curva

Sea $f$ continua en $(a,b)$, si $\forall x_{1};x_{2} \in (a,b); x_{1} \neq x_{2}$, la cuerda que una dichos puntos se encuentra por encima de la curva en (x_{1}, x_{2}) entonces la curva se dirá **convexa**, por el contrario, si la cuerda está por debajo, se dirá **cóncava**.

Por el signo de la derivada segunda, podemos saber si $f$ es cóncava o convexa

Si $f''(x)>0 \forall x \in (a) \implies f(x) es **convexa** en (a,b)$
Si $f''(x)<0 \forall x \in (a) \implies f(x) es **cóncava** en (a,b)$




