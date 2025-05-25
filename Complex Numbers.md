## definition: complex numbers, $\mathbf{C}$
- A complex number is and ordered pair $(a,b)$, where $a,b \in R$, but we will write this as $a + bi$
- The set of all complex numbers is denoted by $\mathbf{C}$:
 $$
 \mathbf{C} = \{a + bi : a,b \in \mathbf{R}\}
 $$
- Addition and multiplication on $\mathbf{C}$ are defined by:
 $$
 \begin{array} \\
 (a + bi) + (c + di) = (a + c) + (b + d)i \\
 (a + bi)(c + di) = (ac - bd) + (ad + bc)i
\end{array}
 $$


## properties of complex arithmetic
- **commutativity**
$$\forall \alpha, \beta \in \mathbf{C}, \quad \alpha + \beta = \beta + \alpha \wedge \alpha \beta = \beta \alpha$$
- **associativity**
$$\forall \alpha, \beta, \lambda \in \mathbf{C} \quad (\alpha + \beta) + \lambda = \alpha + (\beta + \lambda) \ \wedge \ (\alpha \beta)\lambda = \alpha(\beta \lambda)$$
- **identities**
$$\forall \lambda \in \mathbf{C}, \quad \lambda + 0 = \lambda \wedge \lambda 1 = \lambda$$
- **additive inverse**
$$\forall\lambda \in \mathbf{C}, \: \exists! \beta \in \mathbf{C}, \quad \alpha + \beta = 0$$
- **multiplicative inverse**
$$\forall \alpha \in \mathbf{C}, \: \exists!\beta \in \mathbf{C}, \quad \alpha \beta = 1$$
- **distributive property**
$$\forall \lambda, \alpha, \beta \in \mathbf{C}, \quad \lambda(\alpha \beta) = \lambda \alpha + \lambda \beta$$
## definition: list, length
- A list of length $n$ is an ordered collection of $n$ elements
- Two lists are equal if and only if they have the same length and the same elements in the same order

## definition: $\mathbf{F}^n$
$$\mathbf{F}^n = \{ (x_{1}, \ldots, x_{n}): x_{k} \in \mathbf{F}, \ k = 1, \ldots, n\}$$
## Fields
A field is a set containing at least two distinct elements called 1 and 0, along with the complex arithmetic properties listed out above.
## Exercises
### Show that $\alpha + \beta = \beta + \alpha, \quad \forall \alpha, \beta \in \mathbf{C}$
$$
\alpha + \beta = (a + c) + (b + d)i = (c + a) + (d + b)i = c + di + a + bi = \beta + \alpha
$$
### Show that $(\alpha + \beta) + \lambda = \alpha (\beta + \lambda), \quad \forall \alpha, \beta \in \mathbf{C}$
$$
\begin{array} \
(\alpha + \beta) + \lambda = \Bigl[(a + c) + (c + d)i\Bigr] + \lambda = \Bigl[ (a + c) + e \Bigr] + \Bigl[ (b + d) + f \Bigr]i = \\ = (a + c + e) + (b + d + f)i = \ldots = \alpha + (\beta + \lambda)
\end{array}
$$
### Show that $\forall \alpha \in \mathbf{C}, \quad \exists!\beta \in \mathbf{C}, \quad \alpha + \beta = 0$
$$
\begin{array}{l}
\\[-0.6em]
\textbf{(Field axiom for }\mathbf R\textbf{)} \\[0.2em]
\forall x\in\mathbf R,\;\exists!\,y\in\mathbf R,\;x+y=0
\\[1.2em]

\textbf{Apply this to each coordinate} \\[0.2em]
\forall a,b\in\mathbf R,\;\exists!\,(c,d)\in\mathbf R^{2},\;a=-c\;\wedge\;b=-d
\\[1.2em]

\textbf{(Definition of complex addition)} \\[0.2em]
\forall\alpha,\beta\in\mathbf C,\;
\alpha=a+bi,\;\beta=c+di
\\[0.2em]
\alpha+\beta=0
\;\Rightarrow\;
(a+c)+(b+d)i=0
\;\Rightarrow\;
a=-c\;\wedge\;b=-d
\;\Rightarrow\;
\alpha=-\beta
\\[1.2em]

\textbf{Existence.} \\
\text{Choose }c=-a,\;d=-b\text{ and set }\beta=c+di=-a-bi.
\text{ Then } \alpha+\beta=0. \\[0.6em]

\textbf{Uniqueness.} \\
\text{If }\gamma\in\mathbf C\text{ also satisfies }\alpha+\gamma=0,
\text{ write }\gamma=e+fi.\\
\text{The same calculation forces }e=-a,\;f=-b,
\text{ so }\gamma=\beta.
\\[1.2em]

\therefore\;
\forall\alpha\in\mathbf C,\;\exists!\beta\in\mathbf C,\;\alpha+\beta=0.
\end{array}
$$
### Show that $\forall \alpha \in \mathbf{C}, \alpha\neq 0, \: \exists!\beta \in \mathbf{C}, \quad \alpha \beta=1$
$$
\begin{array}{l} \\[-0.6em]
\text{Suppose } \alpha = a + bi \ \wedge \ \beta = c + di \text{ where } a,b,c,d \in \mathbf{R} \\
\text{then } \alpha \beta = 1 \Leftrightarrow (ac - bd) + (ad + bc)i = 1 \\
\text{thus we get a system of equations} \\
\begin{equation}
\begin{cases}
ac - bd = 1 \\
ad + bc = 0
\end{cases}
\end{equation} \\
\text{lets treat c and d as unknowns} \\
\det \begin{pmatrix}
a& -b \\
b& a
\end{pmatrix} = a^2 + b^2 \neq 0 \\
\text{Because determinant is not 0, there exists a unique solution} \\
c = \frac{a}{a^2 + b^2}, \quad d = -\frac{b}{a^2+b^2} \\[0.6em]
\therefore \forall \alpha \in \mathbf{C}, \alpha\neq 0, \: \exists!\beta \in \mathbf{C}, \quad \alpha \beta=1
\end{array}
$$
### Show that $-\frac{1 + \sqrt{3}i}{2}$ is a cube root of 1
$$
\begin{array}{l} \\[-0.6em]
e^{2\pi i} = 1 \\
\sqrt[3]{1} = e^{\frac{2}{3}\pi i} \\
e^{\frac{2}{3}\pi i} = \cos\left( \frac{2}{3}\pi \right) + i \sin\left( \frac{2}{3}\pi \right) = \\
= -\sin\left( \frac{\pi}{6} \right) + i \cos\left( \frac{\pi}{6} \right) = \\
-\frac{1}{2} + \frac{\sqrt{3}i}{2} = - \frac{1 + \sqrt{3}i}{2} \quad \square
\end{array}
$$
### Find two distinct square roots of $i$
$$
\begin{array}{l} \\[-0.6em]
i = e^{\frac{\pi}{2}i} \\
\sqrt{i} = e^{\frac{\pi}{4}i} \ \vee \ \sqrt{i} = e^{\frac{5\pi}{4}i} \\
\sqrt{i} = \frac{\sqrt{2}(i + 1)}{2} \ \vee \ \sqrt{i} = -\frac{\sqrt{2}(i + 1)}{2}
\end{array}
$$
### Find $x \in \mathbf{R}^4$ such that $(4, -3, 1, 7) + 2x = (5, 0, -6, 8)$
$$
\begin{array}{l}
2x = (5 - 4, 0 + 3, -6 - 1, 8 - 7) = (1, 3, -7, 1) \\
x = \left( \frac{1}{2}, \frac{3}{2}, -\frac{7}{2}, \frac{1}{2} \right)
\end{array}
$$

### Explain why there does not exist $\lambda \in \mathbf{C}$ such that $\lambda(2 - 3i, 5 + 4i, -6 + 7i) = (12 - 5i, 7 + 22i, -32 - 9i)$
$$
\begin{align}
&\text{Suppose } \lambda = a + bi \\[0.6em]

&\begin{cases}
\lambda(2 - 3i)& = &12 - 5i \\
\lambda(5 + 4i)& = &7 + 22i \\
\lambda(-6 + 7i)& = & -32 - 9i
\end{cases} \\
\\
&\begin{cases}
(2a + 3b) + (-3a + 2b)i &=& 12 - 5i \\
(5a - 4b) + (4a + 5b)i &=& 7 + 22i \\
(-6a - 7b) + (-7a - 6b)i &=& -32 - 9i
\end{cases} \\
\\
&\begin{cases}
2a + 3b &=& 12 \\
5a - 4b &=& 7 \\
-6a - 7b &=& -32
\end{cases} \\
\\
&a = \frac{12 - 3b}{2} \\ \\
\cdots

\end{align}
$$
