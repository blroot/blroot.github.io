---
published: true
---
Integral triple, cálculo de volúmenes, coordenadas cilíndricas, coordenadas esféricas.

## Integral triple

Así como en las integrales dobles la región de integración elemental es un rectángulo, en las integrales triples al agregar una variable, la regíon resulta en un cubo o paralelepípedo.

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

## Coordenadas esféricas

Es conveniente utilizar este cambio de variables cuando tenemos cuerpos como esferas o conos

De forma general tenemos:

$$
\left\{\begin{aligned}
&x=\rho sin(\phi) cos(\theta) \\
&y=\rho sin(\phi) sin(\theta) \\
&z=\rho cos(\phi)
\end{aligned}
\right.
$$

Ejemplos:

Para obtener una esfera de radio r (dejamos $$\rho$$ constante):

$$
\left\{\begin{aligned}
&\rho = r \\
&0 \le \theta \le 2 \pi \\
&0 \le \phi \le \pi
\end{aligned}
\right.
$$

Para obtener un cono (dejamos $$\phi$$ constante):

$$
\left\{\begin{aligned}
&\rho_{0} \le \rho \le \rho_{1} \\
&0 \le \theta \le 2 \pi \\
&\phi = \frac{\pi}{4}
\end{aligned}
\right.
$$

En todos los casos el jacobiano es 

$$|J|=\rho^2 sin(\phi)$$

Las posibilidades son varias, así que es importante darse cuenta que cuerpo obtenemos según los valores que tomen $$\rho, \phi, \theta$$

<iframe scrolling="no" title="Coordenadas esféricas" src="https://www.geogebra.org/material/iframe/id/b6dmsdhm/width/1920/height/933/border/888888/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="100%" style="border:0px;"> </iframe>
