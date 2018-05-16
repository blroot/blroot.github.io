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
