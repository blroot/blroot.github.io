---
published: true
---
Alguien alguna vez me dijo que aprendemos algo cuando debemos explicarlo. Por eso, la motivación de este tipo de entradas es explicarle a mi alter ego, por supuesto, estaré mas que contento si te encontrás leyendo estas palabras y mucho más si te llevas algo útil. También son bienvenidas las puteadas en caso de que haya dicho alguna burrada, sepan disculpar, no es mi intención ser docente (al menos por el momento)

## Espacios Vectoriales

Bien, vamos a suponer que estamos familiarizados con los espacios euclídeos ($ R^n $) sobretodo $ R^2 $ (plano) y $ R^3 $ (espacio tridimensional) y con algunos de los elementos del álgebra lineal (rectas y planos)

Un espacio vectorial es un cuerpo constituído por dos conjuntos, uno de vectores y otro de escalares, una operación y una acción.

Con $ V = R^n $ (vectores) y $ K = R $ (escalares) a la operación llamémosle suma ($ + $)
y a la acción la llamamos producto por escalar ($ \cdot $)

Un espacio vectorial debe cumplir ciertas propiedades, básicamente los elementos de $ V $ deben poder sumarse entre sí y multiplicarse por los elementos de K

Entonces el espacio queda formado como

$$ (V, K, +, \cdot) \label{eq:spc}$$

Entonces, decimos que $ V $ es un $K$-espacio vectorial

### Un ejemplo

Por ejemplo, sea $ V = R^(2x2) $ y $ K = R $

¿Es $ V $ un $K$-espacio vectorial?

Veamos si se cumple la suma:

$ A \in R^(2x2) $ y $ B \in R^(2x2) => A+B \in R^(2x2) $

Sean $A y B$:

$$ A=\begin{bmatrix}
    a & b \\
	c & d
\end{bmatrix} $$

$$ B=\begin{bmatrix}
    e & f \\
	g & h
\end{bmatrix} $$

$$=> A+B=\begin{bmatrix}
              a+e & b+f \\
              c+g & d+h
\end{bmatrix}$$

Como vemos, $ A+B \in R^(2x2) $

Veamos si se cumple el producto por escalar:

$ A \in R^(2x2) $ y $ k \in R => k\cdot A \in R^(2x2) $

Sea

$$ A=\begin{bmatrix}
    a & b \\
	c & d
\end{bmatrix} $$

$$=> k\cdot A=\begin{bmatrix}
              k*a & k*b \\
              k*c & k*d
\end{bmatrix}$$

Se observa que $ k\cdot A \in R^(2x2) $

Entonces, decimos que $ V $ es un $K$-espacio vectorial
__________
## Subespacio

Sea $V$ un $K$-espacio vectorial y $S\subseteq V$ se dice que $S$ es un subespacio de $V$ si $S$ "hereda" las propiedades de $V$, es decir:

$$ (S, K, +, \cdot) $$ Luego $S$ es un subespacio de $V$

Las propiedades que debe cumplir un subespacio son:

- $\vec{0} \in S$

Es decir el vector nulo pertenece al subespacio

- Con $s_{1},s_{2} \in S => s_{1}+s_{2} \in S$

La suma de vectores pertenecientes a $S$, pertenece a $S$

- Con $s \in S$ y $k \in K => k\cdot s \in S$

El producto de un vector $\vec{s}$ por un escalar $k$ pertenece a $S$

### Ejemplo

$$ W={(x_1, x_2, x_3) \in R^3 / 2x_1-x_2+x_3=0} $$

¿Es $W$ un subespacio de $R^3$?

$(W, K, +, \cdot)$ con $K=R$

Veamos si se cumplen las propiedades

- $\vec{0} \in W$

Es fácil ver que $(0, 0, 0) \in W$
  
  

- Con $\vec{v},\vec{w} \in W => v+w \in W$

Sean:

$$\vec{v}=(v_1, v_2, v_3)$$;
$$\vec{w}=(w_1, w_2, w_3)$$

$=> \vec{v+w}=(v_1+w_1, v_2+w_2, v_3+w_3)$

Ahora reemplazamos en la ecuación que define a $W$ (es un plano)

$$2(v_1+w_1)-(v_2+w_2)+(v_3+w_3)=0$$

Distribuyendo

$$2v_1+2w_1-v_2-w_2+v_3+w_3=0$$

Agrupando los elementos de un mismo vector

$$2v_1-v_2+v_3+2w_1-w_2+w_3=0$$

Por la ecuación, sabemos que 

$$2v_1-v_2+v_3=0$$

$$2w_1-w_2+w_3=0$$

$=> 2v_1-v_2+v_3+2w_1-w_2+w_3=0+0=0$

Por lo tanto se cumple que Con $\vec{v},\vec{w} \in W => \vec{v+w} \in W$
  
  

- Con $\vec{v} \in W$ y $k \in K => k\cdot \vec{v} \in W$

Sea:

$$\vec{v}=(v_1, v_2, v_3)$$

$$k\cdot \vec{v} = (kv_1, kv_2, kv_3)$$

Reemplazamos en la ecuación que define a $W$

$$2kv_1-kv_2+kv_3=0$$

Saco factor común $k$

$$k(2v_1, v_2, v_3)=0$$

Por la ecuación, sabemos que

$$2v_1, v_2, v_3=0$$

Entonces

$$k(0)=0$$ 

Se cumple para todo $k \in K$

Como $W$ cumple las tres propiedades, entonces se dice que $W$ es un subespacio de $R^3$   
  
  
En la segunda parte de espacios vectoriales vamos a ver:

-¿Qué es un generador y por qué nos permite expresar un espacio vectorial?
-Dependencia e independencia lineal  
-Base de un espacio vectorial

[Link a la segunda parte](https://blroot.github.io/Espacios-Vectoriales-2/ "Segunda parte de espacios vectoriales")
