---
published: true
---
Teorema de Green, teorema de Stokes o del rotor, teorema de Gauss o de la divergencia

## Teorema de Green

Dada una curva $$C$$ simple y orientada en forma positiva, encerrando una región $$R$$ en el plano $$xy$$, la integral curvilinea de un campo $$F: D \in \Re^2 \to \Re^2 / F=(P(x,y), Q(x,y))$$ donde $$P,Q$$ son funciones diferenciables en $$\Re$$ se puede calcular mediante:

$$ \oint_{C+} F \cdot dS = \int \int_R (Q'_{x} - P'_{y}) dxdy $$

Si $$F$$ es un campo conservativo, luego, se cumple que $$Q'_{x} - P'_{y}=0 \implies \oint_C+ F \cdot dS = 0$$

## Teorema de Stokes o del rotor

La integral de un campo vectorial $$F: D \in \Re^3 \to \Re^3$$ sobre una curva $$C$$ en $$\Re^3$$ regular, simple y cerrada, resulta igual a la integral del rotacional de dicho campo sobre la superficie encerrada por la curva, siendo $$C$$
Se puede tomar cualquier superficie que contenga a la curva.

$$ \oint_{C+} F \cdot dS = \int \int_{S+} rot(F) \cdot dS $$

## Teorema de Gauss o de la divergencia

### Significado físico de la divergencia

Representa el flujo del campo a través de la superficie en un punto determinado. Siendo el flujo, la cantidad de lineas de campo que atraviesan la superficie por unidad de superficie.

Cuando $$div(F) > 0$$ significa que en el punto calculado el campo emerge de la superficie (fuente)
Cuando $$div(F) < 0$$ significa que en el punto calculado el campo confluye hacia la superficie (sumidero)
Si $$div(F) = 0$$ no hay transferencia de campo entre la superficie y el exterior.

La integral de un campo vectorial $$F: D \in \Re^3 \to \Re^3$$ sobre una superficie cerrada $$S$$ orientada de forma positiva, es igual a la integral triple de la divergencia del campo vectorial sobre el volumen encerrado por la superficie.

$$ \oint \oint_{S+} F \cdot dS = \int \int \int_V div(F) dV $$

