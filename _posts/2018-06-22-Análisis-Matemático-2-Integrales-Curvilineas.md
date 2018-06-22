---
published: true
---
Integral curvilinea, longitud de arco, integral curvilinea de un campo escalar, independencia de la trayectoria, integral curvilinea de un campo vectorial

## Integral curvilinea

Así como ya integramos sobre intervalos (podemos pensar un intervalo como una curva, así que estas son un caso especial de integrales sobre curvas) también deseamos integrar sobre curvas.

## Integral curvilinea de un campo escalar

Por ejemplo:

Sea una curva en $$\Re^2$$ $$C(t)=(x(t), y(t)); t_{0} \le t \le t_{1}$$

Calculamos la integral del campo esscalar $$z=f(x,y)$$ de la siguiente manera:

$$ \int_{t_{0}}^{t_{1}} f(x(t), y(t)) ||C'(t)|| dt $$

Por ejemplo, tomemos la curva $$C(t)=(0, t); 0 \le t \le 4$$

Nos queda

$$ \int_{0}^{4} f(0, t) dt $$

## Longitud de arco

Como ya podemos imaginar, cuando el campo escalar a integrar es constante e igual a 1, la integral nos da como resultado la longitud de arco de la curva.

## Independencia de la trayectoria

## Integral curvilinea de un campo vectorial

Sea un campo vectorial en $$\Re^2$$ o $$\Re^3$$

se calcula la integral curvilinea dichos campos vectoriales de la siguiente manera:

$$ \int_C F \cdot s = \int_{t_{0}}^{t_{1}} F(C(t)) \cdot C'(t) dt $$

### Propiedades

Si $$F$$ es campo gradiente (o conservativo)

1- Si $$C$$ es una curva abierta con extremos A y B, el resultado de la integral es independiente del camino que tomemos para ir desde A hasta B.

2- La integral también se puede calcular a través de la función potencial $$\phi$$

$$\int_C F \cdot ds = \phi_{(B)} - \phi_{(A)}$$

3- Si la curva es cerrada

$$\int_C F \cdot ds = 0$$

Recordemos que para que un campo sea conservativo, se debe cumplir:

En $$\Re^2$$: $$Q'_{x} - P'_{y} = 0$$

En $$\Re^3$$: $$rot(F) = \vec 0$$

Si además de esas condiciones se cumple que $$C$$ es cerrada y la región encerrada por la curva es simplemente conexa, el campo es conservativo en dicho recinto.
Decimos que un recinto es simplemente conexo cuando podemos unir dos puntos A y B de ella con una curva perteneciente al conjunto.



