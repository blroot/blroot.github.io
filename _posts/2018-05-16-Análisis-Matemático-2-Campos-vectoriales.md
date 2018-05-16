---
published: true
---
Definición, lineas de campo, operador nabla, función potencial.

## Definición

LLamamos campo vectorial a una función vectorial $$F:D \subseteq \Re^n \to \Re^n$$

Por ejemplo: $$F:D \subseteq \Re^3 \to \Re^3 / F(x,y,z)=(F_{1}(x,y,z), F_{2}(x,y,z), F_{3}(x,y,z)) $$


## Lineas de campo

Las lineas de campo son curvas en $$\Re^2$$ o $$\Re^3$$ cuyas trayectorias muestran la continuidad de la orientación de los vectores del campo, estas curvas pueden ser abiertas o cerradas y tienen la propiedad de que no se cortan entre si. En cada punto, el vector del campo es tangente a la curva.

Calcular las lineas de campo, implica resolver las siguientes ecuaciones diferenciales:

En $$\Re^2: $$ $$ \frac{dx}{F_{1}} = \frac{dy}{F_{2}}$$

En $$\Re^3: $$ $$ \frac{dx}{F_{1}} = \frac{dy}{F_{2}} = \frac{dz}{F_{3}} $$

Ej: $$F(x,y) = (-y, x)$$

$$F_{1} = -y; F_{2} = x$$

Planteamos la ecuación diferencial:

$$ \frac{dx}{-y} = \frac{dy}{x}  \\
\int \frac{dx}{-y} = \int \frac{dy}{x} \\
\frac{x^2}{2} = \frac{-y^2}{2} + C
\implies x^2+y^2=2C
$$

Entonces las lineas de campo son circunferencias de radio $$\sqrt 2C$$

Ejercicio:

Dado el campo vectorial $$F(x,y,z)=\frac{-y}{z}i-\frac{x}{z}j+\frac{xy}{z^2}k$$
Hallar una parametrización de la linea de campo que pasa por $$P_{0}=(1,1,1)$$

Como se trata de una curva en $$\Re^3$$ va a estar definida por la intersección de dos superficies

Pleanteando la ecuación diferencial:

$$ \frac{dx}{\frac{-y}{z}} = \frac{dy}{\frac{-x}{z}} = \frac{dz}{\frac{xy}{z^2}} $$

de la primera y segunda ecuación:

$$ \frac{dx}{\frac{-y}{z}} = \frac{dy}{\frac{-x}{z}} \\
-xdx = -ydy \\
\int -xdx = \int -ydy \\
\implies x^2-y^2=C_{1}
$$

de la segunda y tercera:

$$ \frac{dy}{\frac{-x}{z}} = \frac{dz}{\frac{xy}{z^2}} \\
\frac{xy}{z^2}dy = \frac{-x}{z}dz \\
\int ydy = \int -zdz \\
\frac{y^2}{2} = \frac{-z^2}{2} + C_{2}
\implies y^2+z^2=C_{2}
$$

Como la curva debe pasar por $$P_{0}$$ podemos averiguar $$C_{1}$$ y $$C_{2}$$

$$ 1^2-1^2=0 \implies C_{1}=0 $$

$$ 1^2+1^2=2 \implies C_{2}=2 $$

Luego nos queda:

$$y^2=x^2 \implies |y|=x $$

$$ y^2=2-z^2 \\
|z| = \sqrt 2-y^2
$$

Luego una parametrización puede ser $$ C(t) = (t,t, \sqrt (2-y^2)) $$