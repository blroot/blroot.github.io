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

Dado el campo vectorial $$F(x,y,z)=\frac{-y}{z}\hat{i}-\frac{x}{z}\hat{j}+\frac{xy}{z^2}\hat{k}$$
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

## Operador nabla

Llamamos así a un pseudovector de componentes derivadas parciales y se define solo para campos en $$\Re^3$$

Si aplicamos el operador a un campo escalar, obtenemos el vector gradiente del campo escalar.

Siendo $$f$$ un campo escalar, entonces $$\nabla f = (\frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z}) = \vec grad(f)$$

Ej: siendo $$f(x,y,z)=x^2y-2z^2cos(x)$$

$$\implies \nabla f = (2x+2z^2sen(x), x^2, -4zcos(x))$$

Aplicado a un campo vectorial, el operador nabla brinda los siguientes resulados

### Divergente de F

$$Div(F) = \nabla \dot F = (\frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z}) \dot (F_{1}, F_{2}, F_{3}) = F'_{1x} + F'_{2y} + F'_{3z} $$

### Rotacional o rotor

$$rot(F) = \nabla X F = 

\left| \begin{array}{ccc}
\hat{i} & \hat{j} & \hat{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
F_{1} & F_{2} & F_{3} \end{array} \right|\ = (F'_{3y}-F'_{2z})\hat{i}-(F'_{3x}-F'_{1z})\hat{j}+(F'_{2x}-F'_{1y})\hat{k}

$$

Cuando las derivadas parciales en un punto existen y son continuas y el rotacionalen dicho punto es $$\vec 0$$ diremos que el campo es irrotacional. A estos campos se los denomina conservativos o gradientes. El término campo gradiente refiere a que el campo vectorial se obtiene a través de una función escalar llamada "potencial".

Ej: $$F(x,y,z)=(2xy, x^2+z^2, 2zy)$$

Comprobar si F es conservativo y hallar su función potencial.

Sabemos que $$fF_{1}, F_{2}, F_{3}$$ tienen derivadas parciales continuas en $$\Re^3$$

calculamos rotacional:

$$rot(F) = \nabla X F = 

\left| \begin{array}{ccc}
\hat{i} & \hat{j} & \hat{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
2xy & x^2+z^2 & 2zy \end{array} \right|\ = (2z-2z)\hat{i}-(0-0)\hat{j}+(2x-2x)\hat{k} = (0,0,0)

$$

Luego el campo es conservativo y existe función potencial.

## Cálculo de la función potencial

Para el ejemplo anterior:

$$ \frac{\partial f}{\partial x} = 2xy $$

$$ \frac{\partial f}{\partial y} = x^2+z^2 $$

$$ \frac{\partial f}{\partial z} = 2zy $$

resolvemos las ecuaciones diferenciales

$$ \int \frac{\partial f} =  \int 2xy{\partial x} \\
f_{1}(x,y,z) = \int 2xydx + g(y,z) + C_{1} \\
f_{1}(x,y,z) = x^2y+g(y,z)+C_{1}
$$

$$ \int \frac{\partial f} =  \int (x^2+z^2){\partial y} \\
f_{2}(x,y,z) = \int (x^2+z^2)dy+h(x,z)+C_{2} \\
f_{2}(x,y,z) = x^2y+z^2+h(x,z)+C_{2}
$$

$$ \int \frac{\partial f} =  \int (x^2+z^2){\partial z} \\
f_{3}(x,y,z) = \int 2zydz+l(x,y)+C_{3} \\
f_{3}(x,y,z) = z^2y+l(x,y)+C_{3}
$$

luego la función potencia queda como:

$$f(x,y,z) = x^2y+z^2y+C$$








