---
published: true
---
## Espacios Vectoriales

Alguien alguna vez me dijo que aprendemos algo cuando debemos explicarlo. Por eso, la motivación de este tipo de entradas es explicarle a mi alter ego, por supuesto, estaré mas que contento si te encontrás leyendo estas palabras y mucho más si te llevas algo útil. También son bienvenidas las puteadas en caso de que haya dicho alguna burrada, sepan disculpar, no es mi intención ser docente (al menos por el momento)

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

Sea $A$
$$ A=\begin{bmatrix}
    a & b \\
	c & d
\end{bmatrix} $$

$$=> k\dot A=\begin{bmatrix}
              k*a & k*b \\
              k*c & k*d
\end{bmatrix}$$

Se observa que $ k\cdot A \in R^(2x2) $

Entonces, decimos que $ V $ un $K$-espacio vectorial








