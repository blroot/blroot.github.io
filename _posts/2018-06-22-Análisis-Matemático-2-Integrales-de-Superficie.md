---
published: true
---
Integrales de superficie, integrales de superficie sobre campos escalares, área de una superficie, integrales de superficie sobre campos vectoriales.

## Integrales de superficie sobre campos escalares

1- Superficie paramétrica $$S(u,v)$$

$$ \int \int_S f(x,y,z) dS = \int \int_{R_{uv}} f(x(u,v), y(u,v), z(u,v)) || S'_{u} \times S'_{v} || dudv $$

2- Superficie implícita $$g(x,y,z)=0$$


$$ \int \int_S f(x,y,z) dS = \int \int_{R_{xy}} f(x,y,z) \frac{||\nabla g||}{|\nabla g \cdot \hat{k}|} dxdy $$

Acá podemos también proyectar sobre los otros planos, deberemos cambiar en ese caso versor k por el correspondiente y cambian las variables de integración.

3- Superficie explícita $$z=g(x,y)$$

$$ \int \int_S f(x,y,z) dS = \int \int_{R_{xy}} f(x,y, g(x,y)) \sqrt((g'_{x})^2 + (g'_{y})^2 + 1) dxdy $$

## Area de una superficie

Como ya estamos acostumbrados, si la función a integrar es f(x,y,z)=1 la integral nos va a dar como resultado el área de la superficie S

## Integrales de superficie sobre campos vectoriales

1- Superficie paramétrica $$S(u,v)$$

$$ \int \int_S F \cdot dS = \int \int_{R_{uv}} f[x(u,v), y(u,v), z(u,v)] \cdot (S'_{u} \times S'_{v}) dudv $$

2- Superficie implícita $$g(x,y,z)=0$$

$$ \int \int_S F \cdot dS = \int \int_{R_{xy}} F(x,y,z) \cdot \nabla g \frac{1}{|\nabla g \cdot \hat{k}|} dxdy $$

Acá podemos también proyectar sobre los otros planos, deberemos cambiar en ese caso versor k por el correspondiente y cambian las variables de integración.

3- Superficie explícita $$z=g(x,y)$$

$$ \int \int_S F \cdot dS = \int \int_{R_{xy}} F(x,y,g(x,y)) \cdot (-g'_{x}, -g'_{y}, 1) dxdy $$

## Propiedad

$$ \int \int_{S+} F \cdot dS = - \int \int_{S-} F \cdot dS $$
