---
published: true
---
## Coordenadas homogeneas

Una de las herramientas del álgebra lineal que se utilizan muy frecuentemente en computación gráfica -tanto en 2D como en 3D- son las coordenadas homogéneas. A continuación vamos a exponer de forma práctica el porqué de su utilización, teóricamente tambíen tiene implicancias proyectivas, pero en un principio es más facil entenderlo de la siguiente manera.

Bien, una de las principales problemáticas geométricas que necesitamos resolver en nuestros programas gráficos es mover objectos, ¿Como movemos objetos? transformando linealmente o de manera afín nuestras primitivas, principalmente vértices en el caso de triángulos, pero dependiendo del algoritmo que usemos tambíen pueden ser centros (esferas) u otro tipo de coordenadas que necesitemos transformar.

Si necesitás un repaso sobre espacios vectoriales y transformaciones lineales

Ahora bien, por lo general las transformaciones que vamos a querer aplicar a nuestros objetos son tres, rotación, translación y escalado.

En tres dimensiones (espacio), supongamos que tenemos tres vértices 

$$v_{1}=(-1,0,0)$$ 
$$v_{2}=(0,1,0)$$ 
$$v_{3}=(1,0,0)$$ 

Supongamos también que dichos vértices forman un triángulo al que queremos escalar de manera no uniforme . la matríz de transformación de escalado en tres dimensiones tiene esta forma:

$$
S =
\begin{bmatrix}
              s_{x} & 0 & 0 \\
              0 & s_{y} & 0 \\
              0 & 0 & s_{z}
\end{bmatrix}
$$ 

Donde en la diagonal principal se encuentran los coeficientes de escalado para cada coordenada. Por lo tanto si yo quiero agrandar mi triángulo dos unidades sobre el eje X y dejarlo como está sobre el eje Y y Z, la matríz quedaría:

$$
S = 
\begin{bmatrix}
              2 & 0 & 0 \\
              0 & 1 & 0 \\
              0 & 0 & 1
\end{bmatrix} =
$$ 

Como ya tenemos la matríz armada, multiplicamos por derecha cada uno de los vértices para aplicarles la transformación. Los vértices ahora van a ser:

$$v_{1}=(-2,0,0)$$ 
$$v_{2}=(0,1,0)$$ 
$$v_{3}=(2,0,0)$$ 

Perfecto! es lo que queríamos.

Pero como somos ambiciosos, ahora vamos a querer rotarlo. La rotación en tres dimensiones debe hacerse sobre un eje pivote, para continuar con la explicación y que sea más amigable vamos a dar solamente la matríz de rotación sobre el eje Z, pero obviamente esto en un programa no es satisfactorio, se puede construír una matríz de rotación a partir de cualquier vector pivote pero es muy larga y complicada https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula

Entonces, la rotación en 3D sobre el eje Z por un ángulo \theta se representa matricialmente:

$$
R_{z} = 
\begin{bmatrix}
              cos(\theta) & -sin(\theta) & 0 \\
              sin(\theta) & cos(\theta) & 0 \\
              0 & 0 & 1
\end{bmatrix} =
$$

Vemos que tampoco habría problema para transformar nuestros vértices uno por uno, multiplicamos por derecha igual que en el caso anterior.

Ahora, veamos que sucede con la translación, esta vez comencemos al revés, lo que queremos obtener al transformar nuestros vértices es algo como:

$$v_{1} =
\begin{bmatrix}
              -2 + t_{x} \\
              0 + t_{y} \\
              0 + t_{z}
\end{bmatrix}
$$

El problema es que no hay ninguna matríz de 3x3 que nos pueda generar el resultado deseado, te invito a que lo pienses un rato.

Entonces ¿Qué hacemos? bueno, simplemente vamos a agregar una dimensión a nuestras matrices y vértices, algo que debemos tener en cuenta en nuestros vectores es que la cuarta coordenada va a ser $1$ si nos referimos a una posición en el espacio o $0$ si nos referimos a una dirección, ya veremos por que.

La matríz de translación nos quedaría de la siguiente manera:

$$ T = 
\begin{bmatrix}
              1 & 0 & 0 & t_{x} \\
              0 & 1 & 0 & t_{y}\\
              0 & 0 & 1 & t_{z}
              0 & 0 & 0 & 1
\end{bmatrix}
$$ 

Nuestros vértices van a quedar como:

$$v_{1}=(-2,0,0,1)$$
$$v_{2}=(0,1,0,1)$$ 
$$v_{3}=(2,0,0,1)$$ 

Si hacemos las cuentas, vamos a obtener el resultado esperado.
Por otro lado, ¿Qué pasa con las direcciones? ¿Tiene sentido transladar una dirección (un vector)? Realmente no tiene sentido, estamos hablando de espacios vectoriales, todo pasa por el orígen.
Entonces para una dirección, por ejemplo $$d=(1,0,0,0)$$ se puede observar que multiplicando por derecha  por la matriz de translación, el vector queda igual.

De la misma manera, con la cuarta dimensión, el escalamiento queda como:

$$ S = 
\begin{bmatrix}
              s_{x} & 0 & 0 & 0\\
              0 & s_{y} & 0 & 0\\
              0 & 0 & s_{z} & 0\\
              0 & 0 & 0 & 1
\end{bmatrix}
$$ 

Y también la rotación:

$$ R_{z} = 
\begin{bmatrix}
              cos(\theta) & -sin(\theta) & 0 & 0\\
              sin(\theta) & cos(\theta) & 0 & 0\\
              0 & 0 & 0 & 1
\end{bmatrix}
$$

Dicho coloquialmente, las coordenadas homogéneas nos permiten transformar de manera uniforme tanto direcciones como posiciones en el espacio.
