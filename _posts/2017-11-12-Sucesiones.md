---
published: false
---
Definición, límite de una sucesión, ejemplos.

### Sucesiones

Una sucesión es una funcíon  $f:\mathbb{N}->R$. Es decir, una funcíón con dominio en los naturales. Por lo general la notación que usamos es: $f(n)=a_{n}$.
Una sucesión se puede pensar como una lista de números escritos en un órden definido:

$$ {a_{1}, a_{2}, a_{3}...a_{n}} $$

Particularmente, en el análisis matemático, nos interesa estudiar las sucesiones infinitas.

Algunas sucesiones se pueden definir con una fórmula para el n-ésimo término, por ejemplo:

$$ a_{n} = n^2 $$

y produce:

$$ {1^2, 2^2, 3^2, 4^2...n^2} $$

### Límite de una sucesión

La única pregunta que nos podemos hacer con respecto al límite de una sucesión es el límite cuando $n$ tiende a $+inf$:

$$ \lim_{n\to +inf} a_{n} $$

### Ejemplos

1
$$ \lim_{n\to +inf} (n^2+1)/(2n^2-3n)=1/2 $$

2
$$ \lim_{n\to +inf} \frac{(n+1)!+n!}{2(n+1)!} \\
=\lim_{n\to +inf} \frac{(n+1)!(1+\frac{n!}{(n+1)!})}{2(n+1)!} \\
=\lim_{n\to +inf} \frac{\frac{n!}{(n+1)!}}{2} = 1/2 $$

3
$$ \lim_{n\to +inf} n^(1/2) = inf^0 ind. \\
=\lim_{n\to +inf} e^(ln(n^(1/2))) \\
=\lim_{n\to +inf} e^(\frac{ln(n)}{n}) \\ $$

CA

$$\lim_{n\to +inf} \frac{ln(n)}{n} $$

Podemos aplicar L'hopital, pero debemos hacerlo pensando en variable real

$$ \lim_{x\to +inf} \frac{ln(x)}{x} $$

Aplicando L'hopital

$$= \lim_{x\to +inf} \frac{1/x}{1} = 0 $$

Como $\mathbb{N} \subset R$ vale también que:

$$ \lim_{n\to +inf} \frac{ln(n)}{n} = 0 $$

$$ \implies \lim_{n\to +inf} e^(\frac{ln(n)}{n}) = e^0 = 1$$


