---
published: true
---
Definición. Polinomio de McLaurin. Error.

### Definición

Sea $f$ una función con las primeras $n+1$ derivadas continuas, se define el polinomio de Taylor de orden $n$ alrededor de $x_{0}$ como:

$$ P_{n}[f, x_{0}] = \sum_{k=0}^n \frac{f^{(k)}(x_{0})}{k!}(x-x_{0})^k $$

$$ = \frac{f(x_{0})}{0!}(x-x_{0})^0 + \frac{f'(x_{0})}{1!}(x-x_{0})^1 + \frac{f''(x_{0})}{2!}(x-x_{0})^2 + ... \\ + \frac{f^{(n)}(x_{0})}{n!}(x-x_{0})^n $$

En general, la idea es aproximar una función por un polinomio.
El polinomio y la función coinciden en las primeras $n$ derivadas evaluadas en $x_{0}$

### Polinomio de McLaurin

Nos referimos al polinomio de McLaurin, como al polinomio de taylor de órden $n$, calculado alrededor de $x_{0)=0$

### Fórmula del error

El error que se comete al aproximar $f(x)$ por $P_{n}[f, x_{0}](x)$ es:

$$ E_{n}(x) = \frac{f^{(n+1)}(\varepsilon)}{(n+1)!}(x-x_{0})^{n+1} $$

Donde $\varepsilon$ está entre $x$ y $x_{0}$

Por ende:

$$ f(x)= P_{n}[f, x_{0}](x) + E_{n}(x) $$

### Ejercicio

Sea $f(x)=1+2x+cos(x)$. Construír el polinomio de McLaurin de orden 4 para $f$ y usarlo para estimar $f(1/3)$. Ver que el error cometido al estimar $f(1/3)$ es menor a $10^{-4}$

Decimos que:

$$ P_{4}[f, 0](x) = \frac{f(0)}{0!}x^0 + \frac{f'(0)}{1!}x^1 + \frac{f''(0)}{2!}x^2 \\
+ \frac{f'''(0)}{3!}x^3 + \frac{f^{(iv)}(0)}{4!}x^4 $$

Calculo $f(0)$ y las derivadas necesarias:

$$ f(0)=2 $$

$$ f'(x)=2-sen(x) \implies f'(0)=2 $$

$$ f''(x)=-cos(x) \implies f''(0)=-1 $$

$$ f'''(x)=sen(x) \implies f'''(0)=0 $$

$$ f^{(iv)}(x)=cos(x) \implies f^{(iv)}(0)=1 $$

Ya calculo la derivada quinta para el error:
$$ f^{(v)}(x)=-sen(x) \implies f^{(v)}(0)=0 $$

Entonces:

$$ P_{4}[f, 0](x) = 2 + 2x - \frac{1}{2}x^2 + 0 + \frac{1}{24}x^4 $$

Ahora estimo $f(1/3)$

$$ P_{4}[f, 0](1/3) = 2 + 2(\frac{1}{3}) - \frac{1}{2}(\frac{1}{3})^2 + 0 + \frac{1}{24}(\frac{1}{3})^4 = \frac{5077}{1944} $$

Acotando el error:
Cuando hablamos de error, estamos hablando de algo positivo, luego, vamos a querer el valor absoluto de $E_{5}$

$$ |E_{5}(1/3)| = |\frac{f^{(v)}(\varepsilon)}{5!}(1/3)^5| = |\frac{-sen(\varepsilon)}{120*243}| \\
= \frac{|-sen(\varepsilon)|}{29160} \le \frac{1}{29160} \lt \frac{1}{10000} $$

Vemos que se cumple que el error es menor a $10^{-4}$















