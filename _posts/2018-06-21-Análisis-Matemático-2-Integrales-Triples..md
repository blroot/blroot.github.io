---
published: true
---
Integral triple, cálculo de volúmenes, coordenadas cilíndricas, cooredenadas esféricas.

## Integral triple

Así como en las integrales dobles la región de integración elemental es un rectángulo, en las integrales triples al agregar una variable, la regío resulta en un cubo o paralelepípedo.

Por ejemplo:

$$ I = \int_{z=0}^{z=c} \int_{y=0}^{y=b} \int_{x=0}^{x=a} f(x,y,z) dxdydz $$

## Cálculo de volúmenes

Cuando la función a integrar es constante e igual a 1, el resultado de la integral triple, es el volúmen de la región de integración.

$$ V = \int \int \int_{V} 1 dxdydz = \int \int_{R_{xy}} \int_{z_0}^{z_1} dxdydz $$

Podemos ver la integral anterior desde la interpretación del volúmen como base por altura, al aplicar este concepto a la integral triple, la descomponemos en una integral doble que nos dará como resultado el área de la región $$R_{xy}$$ de la base y por otro lado aplicando una integral en $$z$$ que nos dará la altura del cuerpo

## Coordenadas cilíndricas

Este cambio de variables suele ser conveniente cuando la proyección del cuerpo en cuestión sobre el plano $xy$ es una circunferencia o elipse.

Para una circunferencia:

$$
\left\{\begin{aligned}
&x=rcos(\theta) \\
&y=rsin(\theta) \\
&z=z
\end{aligned}
\right.
$$

Donde

$$
\left\{\begin{aligned}
&0 \le r \le r_{0} \\
&0 \le \theta \le 2 \pi \\
&z_{0} \le z \le z_{1}
\end{aligned}
\right.
$$

$$|J|=r$$

Como se puede observar, es muy similar a las coordendas polares, solamente se agrega la altura $$z$$

Para una elipse:

$$
\left\{\begin{aligned}
&x=arcos(\theta) \\
&y=brsin(\theta) \\
&z=z
\end{aligned}
\right.
$$

Donde

$$
\left\{\begin{aligned}
&0 \le r \le r_{0} \\
&0 \le \theta \le 2 \pi \\
&z_{0} \le z \le z_{1}
\end{aligned}
\right.
$$

$$|J|=abr$$

