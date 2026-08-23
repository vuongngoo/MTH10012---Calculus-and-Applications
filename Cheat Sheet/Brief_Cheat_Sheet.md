# MTH10012: Calculus and Applications

## Useful Formulas

### Radians to degrees
- $\text{Radians} \times \frac{180}{\pi} = \text{Degrees}$
- $\text{Degrees} \times \frac{\pi}{180} = \text{Radians}$

### Exact Values
| Degrees | $0^\circ$ | $30^\circ$ | $45^\circ$ | $60^\circ$ | $90^\circ$ |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Radians** | $0$ | $\frac{\pi}{6}$ | $\frac{\pi}{4}$ | $\frac{\pi}{3}$ | $\frac{\pi}{2}$ |
| **Sine** | $0$ | $\frac{1}{2}$ | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{3}}{2}$ | $1$ |
| **Cosine** | $1$ | $\frac{\sqrt{3}}{2}$ | $\frac{\sqrt{2}}{2}$ | $\frac{1}{2}$ | $0$ |
| **Tangent** | $0$ | $\frac{\sqrt{3}}{3}$ | $1$ | $\sqrt{3}$ | undefined |

### Engineering Notation
| Value | Prefix | Symbol | Value | Prefix | Symbol |
| :--- | :--- | :--- | :--- | :--- | :--- |
| $10^{12}$ | Terra | T | $10^{-3}$ | Milli | m |
| $10^{9}$ | Giga | G | $10^{-6}$ | Micro | $\mu$ |
| $10^{6}$ | Mega | M | $10^{-9}$ | Nano | n |
| $10^{3}$ | Kilo | k | $10^{-12}$ | Pico | p |

### Logarithmic Laws
- $\log_a a = 1$
- $\log_a 1 = 0$
- $\log_a mn = \log_a m + \log_a n$
- $\log_a m^P = P \log_a m$
- $\log_a \frac{m}{n} = \log_a m - \log_a n$
- $\log_a \frac{1}{n} = -\log_a n$
- $a^{\log_a m} = m$
- $\log_a 0$ cannot exist
- $\log_a$ (negative) cannot exist
- $\log_a m = \log_a n \Rightarrow m = n$
- $\log_a b = \frac{\log_c b}{\log_c a}$
- $\log_a m = n \Leftrightarrow a^n = m$

### Index Laws
- $a^m \times a^n = a^{m+n}$
- $\frac{a^m}{a^n} = a^{m-n}$
- $a^0 = 1$
- $a^{-n} = \frac{1}{a^n}$
- $(a^m)^n = a^{m \times n}$
- $(ab)^n = a^n \times b^n$
- $a^{\frac{1}{n}} = \sqrt[n]{a}$
- $a^{\frac{m}{n}} = (\sqrt[n]{a})^m$
- $a^b = a^c \Rightarrow b = c$

## Numbers, Sets and Functions

### Number Sets and Inequalities
**Number Sets**
- $\mathbb{N}$ - Natural numbers (Positive whole numbers)
- $\mathbb{Z}$ - Set of integers (Both positive and negative whole numbers)
- $\mathbb{Q}$ - Rational numbers (Numbers that can be written as a ratio of two integers)
- $\mathbb{R}$ - All real numbers
- $\mathbb{Q}'$ (or $\mathbb{I}$) - Irrational numbers (Numbers that don't have a terminating decimal e.g., $\pi, e, \sqrt{3}$)

**Inequalities**
If $b > a$ such that $b - a > 0$ then:
- $b > a \Rightarrow b + c > a + c$ for any value of $c$
- $b > a$ and $c > 0 \Rightarrow bc > ac$
- $b > a$ and $c < 0 \Rightarrow bc < ac$
- If an inequality is multiplied by a negative value, the inequality sign flips.

### Set Notation
- $\in$ - Element of number set
- $\notin$ - Not an element of number set
- $\cup$ - Union of number sets, belongs to either or both number sets
- $\cap$ - Intersection of number sets, exclusive to both number sets
- $\emptyset$ - Null
- $'$ or $^c$ - Compliment (Excluding)

### Interval Notation
- $()$ - Not including / Not equal to
- $[]$ - Including / Equal to

### Induction Principle
A property $\mathcal{P}(n)$ is a statement involving elements $n$ either belonging to $\mathbb{N}$ or one of its subsets.
$\mathcal{P}(n)$ is said to be true if it is valid for every value of $n$, otherwise it is false.
Suppose that a property $\mathcal{P}(n)$ is true for $n=1$. Now suppose also that if the property is assumed to be valid for a generic value of $n$, then this results in it also being valid for $n+1$. Then $\mathcal{P}(n)$ is valid for all numbers $n \in \mathbb{N}$.

*Example*:
$\mathcal{P}(n): 1 + 3 + 5 + \dots + (2n - 1) = n^2$
1. Test that the statement is true for $n=1$:
   $\mathcal{P}(1): (2(1) - 1) = (1)^2 \Rightarrow 1 = 1$ (True)
2. Assume $\mathcal{P}(n)$ is true for all $n \in \mathbb{N}$, and test for $n+1$:
   $\mathcal{P}(n+1): 1 + 3 + 5 + \dots + (2n - 1) + (2(n+1) - 1) = (n+1)^2$
   Substitute the LHS of $\mathcal{P}(n)$ into the equation:
   $n^2 + (2n + 1) = (n+1)^2$
3. Evaluate $\mathcal{P}(n+1)$ when $n=1$:
   $\mathcal{P}(1+1): 1^2 + (2(1) + 1) = (1+1)^2 \Rightarrow 4 = 4$ (True).
   Therefore, by mathematical induction, it is true for $n \in \mathbb{N}$.

### TAPE Method
A shorter way to remember induction theorem steps:
- **T**est that the statement is true for $\mathcal{P}(1)$
- **A**ssume that the statement is true for an arbitrary integer $k$ (i.e. $n=k, k \in \mathbb{Z}$)
- **P**rove that $n=k+1$ is true
- **E**valuate that the statement is true by proof of mathematical induction

## Functions
A function is where each y-value has one x-value. Use the vertical line test to determine if it is a function or relation.
- Crosses once: function
- Crosses twice: relation

### One-to-One Functions
Each x-value gives a unique y-value. Use the horizontal line test to determine one-to-one functions.
- Crosses once: one-to-one function (bijective)
- Crosses twice (or more): many-to-one function (non-bijective)

### Inverse Functions
Only applies to one-to-one functions, graphically reflects over $y=x$.
**Finding Inverse functions:**
1. Let $f(x) = y$
2. Swap the positions of $x$ & $y$ ($x \leftrightarrow y$)
3. Rearrange to make $y$ the subject
4. Replace $y$ with $f^{-1}(x)$
5. Write the domain of the function at the end.
*(The range of $f(x)$ is the domain of $f^{-1}(x)$ and vice-versa)*.

## Trigonometric Functions and Their Identities

### Arc Length and Area of a Curve
- Arc Length: $S = r\theta$
- Area: $A = \frac{1}{2}r^2\theta$
*(Where $\theta$ is in Radians)*

### Other Trigonometric Functions
- $\sec x = \frac{1}{\cos x}$
- $\csc x = \frac{1}{\sin x}$
- $\cot x = \frac{\cos x}{\sin x} = \frac{1}{\tan x}$

### Pythagorean Trigonometric Identities
- $\sin^2 x + \cos^2 x = 1$
- $\sec^2 x - \tan^2 x = 1$
- $\csc^2 x - \cot^2 x = 1$ 

### Double Angle Formulae
- $\sin 2x = 2 \sin x \cos x$
- $\cos 2x = \cos^2 x - \sin^2 x$
- $\cos 2x = 2 \cos^2 x - 1$
- $\cos 2x = 1 - 2 \sin^2 x$

### Sum and Difference of Trigonometric Functions
- $\sin(a \pm b) = \sin a \cos b \pm \cos a \sin b$
- $\cos(a \pm b) = \cos a \cos b \mp \sin a \sin b$

### Hyperbolic Functions
- $\sinh x = \frac{1}{2}(e^x - e^{-x})$
- $\cosh x = \frac{1}{2}(e^x + e^{-x})$
- $\tanh x = \frac{\sinh x}{\cosh x} = \frac{e^x - e^{-x}}{e^x + e^{-x}}$

## Limits of a Function and Continuity

### Concept of a Limit
For an arbitrary value $a$ and limit $L$, we say a function has the limit $L$ as $x$ approaches $a$:
$$ \lim_{x \to a} f(x) = L $$

### One Sided Limits
- Left-hand limit: $\lim_{x \to a^-} f(x) = L_1$
- Right-hand limit: $\lim_{x \to a^+} f(x) = L_2$
If they are different, the double-sided limit does not exist.

### Continuity and Discontinuity of Functions
A function is continuous if:
$$ \lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x) = f(a) $$
If not, it is discontinuous. Types of discontinuity: **Jump, Essential, Removable**.

### Limit Laws
- $\lim [f(x) \pm g(x)] = L_1 \pm L_2$
- $\lim [c \cdot f(x)] = c \cdot L_1$
- $\lim [f(x) \cdot g(x)] = L_1 \cdot L_2$
- $\lim \left[\frac{f(x)}{g(x)}\right] = \frac{L_1}{L_2}$ (where $L_2 \neq 0$)
- $\lim_{x \to a} c = c$
- $\lim_{x \to a} x = a$

### Limits at Infinity
- $\lim_{x \to \infty} \frac{1}{x} = 0$, $\lim_{x \to -\infty} \frac{1}{x} = 0$
- $\lim_{x \to \infty} e^{-x} = 0$, $\lim_{x \to -\infty} e^{-x} = \infty$

### Indeterminate Forms
Forms like $(\frac{0}{0})$, $(\frac{\infty}{\infty})$, or $(\infty - \infty)$.
To solve, factorise (e.g. difference of perfect squares), rationalise (multiply by conjugate), or use standard limits / L'Hôpital's Rule.

### Sandwich Theorem
If $g(x) \le f(x) \le h(x)$ and $\lim_{x \to a} g(x) = \lim_{x \to a} h(x) = L$, then $\lim_{x \to a} f(x) = L$.

### Standard Limits
1. $\lim_{x \to 0} \frac{\sin x}{x} = 1$
2. $\lim_{x \to 0} \frac{1 - \cos x}{x^2} = \frac{1}{2}$
3. $\lim_{x \to 0} \frac{e^x - 1}{x} = 1$
4. $\lim_{x \to 0} \frac{\sqrt{1+x} - 1}{x} = \frac{1}{2}$
5. $\lim_{x \to 0} \frac{\ln(1+x)}{x} = 1$
6. $\lim_{x \to 0^+} x \log_a x = 0$ (for $a > 0$)
7. $\lim_{x \to 0^+} x^x = 1$
8. $\lim_{x \to \infty} (1 + \frac{\alpha}{x})^x = e^\alpha$ (for any $\alpha \in \mathbb{R}$)

### Race to Infinity
Ranking functions by how fast they approach infinity:
1. $x^x$
2. $2^x$ (or $e^x$, $a^x$)
3. $x^2$
4. $x$
5. $\ln x$
*(Constants and periodic functions like $\sin x, \cos x$ never reach infinity.)*

## Sequences

### Definition and Limits
A sequence $(a_n)$ is an ordered set of elements for $n \in \mathbb{N}$.
- **Convergent**: $\lim_{n \to \infty} a_n = L$ (finite)
- **Divergent**: $\lim_{n \to \infty} a_n = \infty$
- **Irregular**: Limit does not exist and doesn't diverge (e.g., oscillating).

### Increasing and Decreasing Sequences
Let $\delta_n = a_{n+1} - a_n$.
- $\delta_n < 0$: strictly decreasing
- $\delta_n > 0$: strictly increasing

### Standard Limits for Sequences
1. $\lim_{n \to \infty} r^n = 0$ (for $|r| < 1$)
2. $\lim_{n \to \infty} a^{\frac{1}{n}} = 1$ (for $a > 0$)
3. $\lim_{n \to \infty} n^{\frac{1}{n}} = 1$
4. $\lim_{n \to \infty} \left(1 + \frac{\alpha}{n}\right)^n = e^\alpha$
5. $\lim_{n \to \infty} \frac{a^n}{n!} = 0$ (for $a > 0$)
6. $\lim_{n \to \infty} \frac{\log_a n}{n^P} = 0$ (for $a, P > 0$)
7. $\lim_{n \to \infty} \frac{n^P}{a^n} = 0$ (for $a, P > 0$)
8. $\lim_{n \to \infty} \frac{n!}{n^n} = 0$

## Differentiation

### First Principles
$$ f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h} $$

### Standard Derivatives
| $f(x)$ | $f'(x)$ | $f(x)$ | $f'(x)$ |
| :--- | :--- | :--- | :--- |
| $c$ | $0$ | $\sin x$ | $\cos x$ |
| $x^n$ | $nx^{n-1}$ | $\cos x$ | $-\sin x$ |
| $e^x$ | $e^x$ | $\tan x$ | $\sec^2 x$ |
| $\ln x$ | $\frac{1}{x}$ | $\sinh x$ | $\cosh x$ |
| $a^x$ | $(\ln a)a^x$ | $\cosh x$ | $\sinh x$ |
| | | $\tanh x$ | $\text{sech}^2 x$ |

### Inverse Trigonometric Functions
| $f(x)$ | $f'(x)$ | Condition |
| :--- | :--- | :--- |
| $\arcsin x$ | $\frac{1}{\sqrt{1-x^2}}$ | $|x| < 1$ |
| $\arccos x$ | $\frac{-1}{\sqrt{1-x^2}}$ | $|x| < 1$ |
| $\arctan x$ | $\frac{1}{1+x^2}$ | |
| $\text{arccot } x$ | $\frac{-1}{1+x^2}$ | |
| $\text{arcsec } x$ | $\frac{1}{|x|\sqrt{x^2-1}}$ | $|x| > 1$ |
| $\text{arcsinh } x$| $\frac{1}{\sqrt{x^2+1}}$ | |
| $\text{arccosh } x$| $\frac{1}{\sqrt{x^2-1}}$ | $x > 1$ |
| $\text{arctanh } x$| $\frac{1}{1-x^2}$ | $|x| < 1$ |

### Rules of Differentiation
- **Chain Rule**: $f(g(x))' = f'(g(x)) \cdot g'(x)$
- **Product Rule**: $(uv)' = u'v + uv'$
- **Quotient Rule**: $\left(\frac{u}{v}\right)' = \frac{vu' - uv'}{v^2}$
- **Derivative of Inverse**: $(f^{-1})'(b) = \frac{1}{f'(a)}$ where $a = f^{-1}(b)$
- **Implicit Differentiation**: Differentiate both sides wrt $x$, applying chain rule to $y$ (yielding $\frac{dy}{dx}$), then rearrange to solve for $\frac{dy}{dx}$.

### Stationary Points & Concavity
- **Stationary Point**: $f'(x) = 0$
- **Second Derivative Test**:
  - $f''(x) > 0 \Rightarrow$ Local Minimum (Convex / Concave Up)
  - $f''(x) < 0 \Rightarrow$ Local Maximum (Concave / Concave Down)
  - $f''(x) = 0 \Rightarrow$ Possible Point of Inflection (check for sign change in $f''(x)$)

### L'Hôpital's Rule
Used for limits resulting in $(\frac{0}{0})$ or $(\frac{\infty}{\infty})$.
$$ \lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)} = L $$

### Taylor's Formula
$$ f(x) \approx f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \dots + \frac{f^{(n)}(a)}{n!}(x-a)^n $$
Lagrange Remainder: $R_{n+1}(x; a) = f(x) - P_n(x)$

## Antidifferentiation and Integration

### Standard Integrals
- $\int kx^n \, dx = k \frac{x^{n+1}}{n+1} + C$ ($n \neq -1$)
- $\int \frac{k}{x} \, dx = k \ln|x| + C$
- $\int (ax+b)^n \, dx = \frac{(ax+b)^{n+1}}{a(n+1)} + C$
- $\int e^{kx} \, dx = \frac{1}{k}e^{kx} + C$
- $\int a^x \, dx = \frac{a^x}{\ln a} + C$

### Trigonometric Integrals
- $\int \sin x \, dx = -\cos x + C$
- $\int \cos x \, dx = \sin x + C$
- $\int \sec^2 x \, dx = \tan x + C$
- $\int \csc^2 x \, dx = -\cot x + C$
*(Same pattern applies to hyperbolic functions, e.g., $\int \sinh x \, dx = \cosh x + C$)*

### Integration by Substitution
Identify an "inner" function $u(x)$, let $du = u'(x) dx$, perform the substitution to simplify the integral, evaluate, and substitute back.

### Integration of Products of Powers of Trig Functions
For $\int \sin^m x \cos^n x \, dx$:
- If $m$ or $n$ is **odd**, break off one term and use $\sin^2 x + \cos^2 x = 1$ to substitute ($u = \cos x$ or $u = \sin x$).
- If $m$ and $n$ are **even**, use double angle formulas: $\sin^2 x = \frac{1}{2}(1 - \cos 2x)$ and $\cos^2 x = \frac{1}{2}(1 + \cos 2x)$.

### Products with Different Arguments
Use identities to convert products to sums/differences:
- $\sin x \cos y = \frac{1}{2}(\sin(x-y) + \sin(x+y))$
- $\cos x \cos y = \frac{1}{2}(\cos(x-y) + \cos(x+y))$
- $\sin x \sin y = \frac{1}{2}(\cos(x-y) - \cos(x+y))$

### Integration by Partial Fractions
Used for rational functions $\frac{p(x)}{q(x)}$.
| Factor in Denominator | Partial Fraction Term |
| :--- | :--- |
| $(x-a)$ | $\frac{A}{(x-a)}$ |
| $(x-a)^m$ | $\frac{A_1}{(x-a)} + \dots + \frac{A_m}{(x-a)^m}$ |
| $(x^2+px+q)$ | $\frac{Bx+C}{(x^2+px+q)}$ |

### Trigonometric and Hyperbolic Substitutions
| Integrand Contains | Substitution | Derivative ($dx$) |
| :--- | :--- | :--- |
| $\sqrt{a^2 - x^2}$ | $x = a \sin \theta$ | $dx = a \cos \theta \, d\theta$ |
| $\sqrt{x^2 + a^2}$ | $x = a \sinh t$ | $dx = a \cosh t \, dt$ |
| $\sqrt{x^2 - a^2}$ | $x = a \cosh t$ | $dx = a \sinh t \, dt$ |

### Integration by Parts
$$ \int u \, dv = uv - \int v \, du $$
Choose $u$ based on priority: **L**ogarithmic, **I**nverse Trig, **A**lgebraic, **T**rigonometric, **E**xponential.

### The Definite Integral and Area
- Definite integral: $\int_a^b f'(x) \, dx = f(b) - f(a)$
- Area above x-axis: $\int_a^b f(x) \, dx$
- Area below x-axis: $-\int_a^b f(x) \, dx$
- Area between curves: $\int_a^b (f(x) - g(x)) \, dx$ (where $f(x) \ge g(x)$)
- Arc length: $L = \int_a^b \sqrt{1 + (f'(x))^2} \, dx$

## Differential Equations (ODEs)
- **Order**: Highest derivative present.
- **Degree**: Highest power to which the highest derivative is raised.

### Separable DEs
$\frac{dy}{dx} = M(x)N(y) \Rightarrow \int \frac{1}{N(y)} \, dy = \int M(x) \, dx$

### First Order Linear DE (Integrating Factor)
Form: $\frac{dy}{dx} + \mathcal{P}(x)y = \mathcal{Q}(x)$
1. Find integrating factor: $J(x) = e^{\int \mathcal{P}(x) \, dx}$
2. Solution: $y(x) = \frac{1}{J(x)} \int \mathcal{Q}(x)J(x) \, dx$

### Second Order Linear ODEs (Constant Coefficients)
Form: $a\frac{d^2y}{dx^2} + b\frac{dy}{dx} + cy = \mathcal{R}(x)$

**Homogeneous Case ($\mathcal{R}(x) = 0$):**
Characteristic equation: $am^2 + bm + c = 0$
1. **Two distinct real roots ($m_1, m_2$)**: $y_H = Ae^{m_1x} + Be^{m_2x}$
2. **One repeated root ($m$)**: $y_H = e^{mx}(A + Bx)$
3. **Complex roots ($\alpha \pm j\beta$)**: $y_H = e^{\alpha x}(A \cos \beta x + B \sin \beta x)$

**Inhomogeneous Case ($\mathcal{R}(x) \neq 0$):**
General solution: $y(x) = y_H(x) + y_P(x)$
Find particular solution $y_P(x)$ using the **Method of Undetermined Coefficients**:
- If $\mathcal{R}(x) = P_n(x)$ (polynomial), try $y_P = A_n x^n + \dots + A_0$.
- If $\mathcal{R}(x) = ke^{px}$, try $y_P = Ce^{px}$.
- If $\mathcal{R}(x) = k \sin qx$ or $k \cos qx$, try $y_P = C \cos qx + D \sin qx$.
*(Multiply by $x$ or $x^2$ if the guessed form overlaps with the homogeneous solution).*

## Functions of Two Variables

### Partial Derivatives
- $f_x = \frac{\partial f}{\partial x}$ (treat $y$ as a constant)
- $f_y = \frac{\partial f}{\partial y}$ (treat $x$ as a constant)
- Mixed derivatives: $f_{xy} = f_{yx}$ (if continuous)

### Chain Rule for Two Variables
If $z = f(x(t), y(t))$:
$$ \frac{dz}{dt} = \frac{\partial z}{\partial x} \cdot \frac{dx}{dt} + \frac{\partial z}{\partial y} \cdot \frac{dy}{dt} $$
If $x$ and $y$ depend on $u, v$:
$$ \frac{\partial z}{\partial u} = \frac{\partial z}{\partial x} \frac{\partial x}{\partial u} + \frac{\partial z}{\partial y} \frac{\partial y}{\partial u} $$

### Stationary Points & Second Derivative Test
Conditions for stationary point: $\frac{\partial f}{\partial x} = 0$ and $\frac{\partial f}{\partial y} = 0$.
Hessian function:
$$ H = \left(\frac{\partial^2 f}{\partial x^2}\right)\left(\frac{\partial^2 f}{\partial y^2}\right) - \left(\frac{\partial^2 f}{\partial x \partial y}\right)^2 $$
- $H > 0$ and $f_{xx} < 0 \Rightarrow$ Local Maximum
- $H > 0$ and $f_{xx} > 0 \Rightarrow$ Local Minimum
- $H < 0 \Rightarrow$ Saddle Point
- $H = 0 \Rightarrow$ Inconclusive
