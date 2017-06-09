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
$$ S+T=v \in V / v=s+t, s \in S, t \in T $$

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

Sean $V=R^3$  
y  
$$ S=(x,y,z) \in R^3 / x=z=0 $$  
$$ T=(x,y,z) \in R^3 / y=z=0 $$  

Obtenemos una base de $S$

$(0,y,0)=y(0,1,0)$  
Base de $S=\{(0,1,0)\}$

Obtenemos una base de $T$

$(x,0,0)=x(1,0,0)$  
Base de $T=\{(1,0,0)\}$

Entonces las bases generan a $S+T$

$$ S+T=gen\{(0,1,0),(1,0,0)\} $$ 

Como sabemos que es linealmente independiente, decimos que es base de $S+T$

Base $S+T=\{(0,1,0),(1,0,0)\}$

### Suma directa

Decimos que $S+T$ es suma directa si y solo si $S \cap T={\vec{0}}$  
Es decir, es suma directa si en la intersección, solo se encuentra el vector nulo.  
Se escribe como $S \bigoplus T$

Una igualdad que nos sirve para saber si la suma es directa sin necesidad de calcular la intersección es la siguiente:  

$$ dim(S+T) = dimS + dimT - dim(S \cap T) $$

En el ejemplo anterior  

$$ 2 = 1 + 1 -dim(S \cap T) $$

Luego, $dim(S \cap T)=0$, entonces la suma es directa

### Un ejercicio para pensar

Sean  

$$ S=x \in R^3 / x_{1}+x_{2}-x_{3}=0 $$
$$ T={(0,-1,1),(2,1,1)} $$  

Hallar $v \in S+T / v \notin S \wedge v \notin T$

Es decir, encontrar todos los vectores $v$ que pertenecen al subespacio $S+T$ pero no a $S$ ni a $T$  
¿Interesante no?

Bien, como primera instancia, me puede llegar a interesar ver como son $S$ y $T$. $S$ es un plano y al parecer $T$ también lo es, ya que es una base de dimensión dos.  
Quiero saber como son estos planos entre sí, para eso busco la ecuación de $T$  

$$ T = \alpha_{1}(0,-1,1)+ \alpha_{2}(2,1,1)=(x,y,z) $$

Triangulando la matriz, obtengo que $x-y-z=0$ para que el sistema no sea incompatible, luego esa es la ecuación del plano.  

Ahora, veo como es la intersección entre ellos

$$
\left| \begin{array}{ccc}
\hat{i} & \hat{j} & \hat{k} \\
1 & 1 & -1 \\
1 & -1 & -1 \end{array} \right|\ = (-2,0,-2)] 
$$  

Bien, entonces intersectan en una recta.
Detengamonos un momento a imaginar como son esos dos espacios vectoriales















