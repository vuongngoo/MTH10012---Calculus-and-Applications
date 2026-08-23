
A property $\mathcal{P}(n)$ is a statement involving elements $n$ either belonging to $\mathbb{N}$ or one of its subsets.

$\mathcal{P}(n)$ is said to be **true** if it is valid for every value of $n$; otherwise, it is **false**.

Suppose that a property $\mathcal{P}(n)$ is true for $n=1$. Now suppose also that if the property is assumed to be valid for a generic value of $n$, then this results in it also being valid for $n+1$.

Then $\mathcal{P}(n)$ is valid for all numbers $n\in\mathbb{N}$.

---

## Example

Let $\mathcal{P}(n)$ be a property of $n\in\mathbb{N}$:

$$
\mathcal{P}(n):\quad 1+3+5+\cdots+(2n-1)=n^2
$$

### 1. Test $\mathcal{P}(1)$

$$
\mathcal{P}(1):\quad 2(1)-1=(1)^2
$$

$$
2-1=1
$$

$$
1=1\implies \text{True}
$$

### 2. Assume $\mathcal{P}(n)$ is true

Assume that:

$$
1+3+5+\cdots+(2n-1)=n^2
$$

We need to show that $\mathcal{P}(n+1)$ is also true:

$$
1+3+5+\cdots+(2n-1)+(2(n+1)-1)=(n+1)^2
$$

Simplifying:

$$
1+3+5+\cdots+(2n-1)+(2n+1)=(n+1)^2
$$

Since the left-hand side of $\mathcal{P}(n)$ is still present, substitute:

$$
n^2+(2n+1)=(n+1)^2
$$

### 3. Prove $\mathcal{P}(n+1)$

Evaluate $\mathcal{P}(n+1)$ when $n=1$:

$$
\mathcal{P}(1+1):\quad 1^2+2(1)+1=2^2
$$

$$
1+2+1=4
$$

$$
4=4\implies \text{True}
$$

Therefore, by the **principle of mathematical induction**:

$$
\boxed{1+3+5+\cdots+(2n-1)=n^2}
$$

is true for all $n\in\mathbb{N}$.

---

## TAPE Method

A shorter and easier way to remember how to use the induction theorem is the **T.A.P.E. method**.

### T — Test

Test that the statement is true for $\mathcal{P}(1)$.

### A — Assume

Assume that the statement is true for an arbitrary integer $k$:

$$
n=k,\quad k\in\mathbb{Z}
$$

### P — Prove

Prove that:

$$
n=k+1
$$

is true.

### E — Evaluate

Evaluate that the statement is true by proof of mathematical induction.

> **Note:** $n=k+1$ is the same as assuming $\mathcal{P}(n+1)$; it just uses different notation.
