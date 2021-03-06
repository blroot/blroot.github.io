---
published: true
---
Definición, Pensando sobre series, Sumas parciales, Convergencia y Divergencia, Serie geométrica, Serie telescópica, Serie alternada, Serie P, Criterios de convergencia.

## Series

Una serie se puede entender como una suma de una sucesión. las series que nos van a interesar son las series infinitas.

Pensemos en el siguiente caso:

Supongamos que enfrente nuestro tenemos una pared, a exactamente 2 metros de distancia, vamos a comenzar a avanzar pero cada vez que damos un paso, avanzamos la mitad de la distancia avanzada anteriormente. Digamos que en el primer paso avanzamos 1 metro.

Entonces pensamos una sucesión:

$$ a_{n} = 1m, 1/2m, 1/4m, 1/8m, ... = \frac{1}{2^{n-1}} $$

Luego, la distancia avanzada luego de 8 pasos:

$$ 1+1/2+1/4+1/8 $$

Hasta ahora nada demasiado interesante. Una pregunta que nos podemos hacer es ¿Vamos a llegar a la pared? Para eso, vamos a plantear la serie infinita como:

$$ \sum_{n=0}^\infty (\frac{1}{2})^{n} $$

Ahora, para obtener la distancia total recorrida, necesitamos una manera de obtener la suma de la serie (más adeltante veremos con detalle la fórmula):

$$ S_{N} =  \frac{1}{1-\frac{1}{2}} = 2m $$

Es decir, en total avanzamos 2 metros, por ende vamos a llegar a la pared.
En este caso, "sumar infinitos números" da algo finito pero esto no siempre es así.

Sintetizando:

Si $a_{n}$ es una sucesión infinita, luego $\sum_{n=0}^\infty a_{n}$ es una serie infinita.

### Sumas parciales

Dada una sucesión a_{n}, definimos la suma parcial de la misma como

$$ S_{N} =  \sum_{n=1}^N a_{n} $$

Decimos que:

$$ \sum_{n=1}^N a_{n}$$ es convergente si $$\lim_{N\to +\infty} S_{N}=L \in R$$
$$ \sum_{n=1}^N a_{n}$$ es divergente si $$\lim_{N\to +\infty} S_{N}=inf$$
$$ \sum_{n=1}^N a_{n}$$ es oscilante si $$\nexists \lim_{N\to +\infty} S_{N}$$

Ej:

$$\sum_{n=0}^\infty \frac{1}{1-1/2} = 2 \implies$$ convergente.
$$\sum_{n=0}^\infty 1 = inf \implies$$ divergente.
$$\sum_{n=1}^\infty (-1)^n$$ oscilante (-1 si N es impar, 0 si N es par).

### Convergencia y divergencia

Condición necesaria para convergencia

Si una serie $\sum a_{n}$ converge $\implies \lim_{n\to +\infty} a_{n}=0$

Cuidado! Esta condición no es recíproca, es decir, que el límite de cero no significa que la serie converge.

Luego también, si $\lim_{n\to +\infty} a_{n} \neq 0 \implies \sum a_{n}$ diverge.

### Serie geométrica

Tiene la forma

$$ \sum_{n=0}^\infty ar^n $$

Llamamos razón geométrica a $r$

Si 
$$|r| \geq 1$$ la serie diverge.

Si 
$$|r| < 1$$ la serie converge y su suma está dada por $$\frac{a}{1-r}$$

### Serie P (de términos positivos)

Tiene la forma

$$ \sum_{n=1}^\infty \frac{1}{n^P} $$

Si
$$-\infty<p\leq 1$$ la serie diverge.

Si
$$ p>1$$ la serie converge.

### Serie alternada

Son aquellas series que alternan en signo, ej:

$$ \sum_{n=0}^\infty (-1)^n a_{n} $$

Estas series convergen si verifican estas condiciones:

1) $$0<a_{n+1}<a_{n} \forall n$$ es decir, es decreciente para todo n

2) $$\lim_{n\to +\infty} a_{n}=0$$

## Otros criterios de convergencia

### Para series de términos positivos

### Criterio integral

Si $$f>0$$, continua y decreciente para $$x \geq 1$$ y $$a_{n}=f(n)$$ luego:

$$ \sum_{n=1}^\infty a_{n}$$ y $$ \int_{1}^\infty f(x) $$

Convergen las dos o divergen las dos.

### Criterio de comparación directa

Sean $$ b_{n} \geq a_{n} >0 \forall n \geq 1 $$

Si $$ \sum_{n=1}^\infty b_{n} $$ converge $$ \implies \sum_{n=1}^\infty a_{n} $$ converge.
Si $$ \sum_{n=1}^\infty a_{n} $$ diverge $$ \implies \sum_{n=1}^\infty b_{n} $$ diverge.

En palabras, si la mayor converge, la menor converge. Y si la menor diverge, la mayor diverge.

### Criterio de comparación en el límite

Sean $$ a_{n}, b_{n}>0 $$ y $$ \lim_{n\to +\infty} \frac{a_{n}}{b_{n}}=L $$ con $$ L \in R>0 $$

Luego, $$\sum_{n=1}^\infty a_{n}$$ y $$\sum_{n=1}^\infty b_{n}$$ ambas convergen o divergen.

### Para series de términos no nulos

### Criterio de D'Alambert

Sea $$\sum a_{n}$$

Calculando $$ \lim_{n\to +\infty} \frac{a_{n+1}}{a_{n}}=L $$

También se puede evaluar absolutamente.

Si:

$$L<1$$ la serie converge.

$$L>1$$ la serie diverge.

$$L=1$$ El criterio no decide.

### Criterio de Cauchy

Sea $$\sum a_{n}$$

Calculando $$ \lim_{n\to +\infty} \sqrt[n] a_{n}=L $$

También se puede evaluar absolutamente.

Si:

$$L<1$$ la serie converge.

$$L>1$$ la serie diverge.

$$L=1$$ El criterio no decide.
