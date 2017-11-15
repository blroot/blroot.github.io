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

### Acotando el error

El error que se comete al aproximar $f(x)$ por $P_{n}[f, x_{0}](x)$ es:

$$ E_{n}(x) = \frac{f^{(n+1)(\varepsilon)}}{(n+1)!}(x-x_{0})^{n+1} $$

Donde $\varepsilon$ está entre $x$ y $x_{0}$

Por ende:

$$ f(x)= P_{n}[f, x_{0}](x) + E_{n}(x) $$




