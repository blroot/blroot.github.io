---
published: true
---
## Operaciones con subespacios

### Intersección de subespacios

Sea $V$ un espacio vectorial y $S$ y $T$ subespacios de V
la intersección de $S$ y $T$ está dada por  
$$ S \cap T=veV / v \in S \wedge v \in T $$

Es decir, todos los vectores de $V$ que existen al mismo tiempo en $S$ y $T$
Así también, la intersección es un subespacio de $V$

### Ejemplo

Sean $U$,$V$ $\subset R^3 /$  
$$ U=X \in R^3 / 2x+3y+z=0 $$
$$ V=X \in R^3 / x+2y-z=0 $$

Entonces planteamos

$$ U \cap V=X \in R^3 / 2x_1+3x_2+x_3=0 \wedge x_1+2x_2-x_3=0 $$

Como podemos observar, se resuelve con un sistema de ecuaciones lineales.
En este caso en particular, como los subespacios son planos, también se puede hacer el producto vectorial con un vector normal de cada plano, de esa manera obtenemos un vector director de la recta (si es que intersectan en una recta) en donde intersectan los dos subespacios.

Como me aburro de hacer sistemas lineales, vamos a hacer el producto vectorial

Las opciones obvias de vectores normales (y que salen de la ecuación implícita) a los planos son  

$v_{u}=(2,3,1)$  
$v_{v}=(1,2-1)$

$$
\left| \begin{array}{ccc}
\hat{i} & \hat{j} & \hat{k} \\
2 & 3 & 1 \\
1 & 2 & -1 \end{array} \right|\ = (-5,3,1)] 
$$

Entonces, $U$ y $V$ intersectan en una recta. Pero lo que queremos es ver que $U\capV$ es un subespacio, entonces vamos a dar el resultado como una base.

Base de $U \cap V=\{(-5,0,1)\}$

Cuidado, también puede suceder que $U$ y $V$ sean el mismo plano, en ese caso los vectores normales de estos planos van a ser paralelos y el producto vectorial va a dar vector nulo $(0,0,0)$, esto no significa que no haya intersección!$

### Suma de subespacios

Sea $V$ un E.V y $S$ y $T$ subespacios de $V$ 
$$ S+T=v\inV / v=s+t, s\inS, t\inT $$

Intentemos ponerlo en palabras:
1.La suma de subespacios se compone por vectores $v$ pertenecientes a $V$
2.Los vectores $v$ son resultado de la suma de dos vectores $s$ y $t$
3.$s$ y $t$ salen de los subespacios $S$ y $T$ respectivamente

Así también, la suma es un subespacio de $V$

Veamos una propiedad que nos va a servir para sumar subespacios

Sean:  
Base de $S=\{v_{1}, v_{2}...v_{r}\}$
Base de $T=\{t_{1}, t_{2}...t_{k}\}$  

Entonces  
$$ S+T=gen{v_{1}, v_{2}...v_{r}, t_{1}, t_{2}...t_{k}} $$  

Como en cualquier E.V si el conjunto es linealmente independiente, es base de $S+T$

### Ejemplo










