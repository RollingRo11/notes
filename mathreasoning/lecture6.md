# Lecture 6  1/28/2025

## Recall the definition of the biconditional $p \Leftrightarrow q=$
To prove $p \Leftrightarrow q$, we prove both $p \Rightarrow q$ and its converse $q \Rightarrow p$.

> [!TIP] **Proposition 1**
> For every integer $x, x$ is odd if and only if $x-1$ is even.

## Proof
**$(\Rightarrow)$ If $x$ is odd, then...**
- $x = 2n+1$ for some $n \in \mathbb{Z}$
- $x-1 = 2n$
- $x-1$ is even

**$(\Leftarrow)$ Conversely, if $x-1$ is even, then...**
- $x = 2n$ for some $n \in \mathbb{Z}$
- $x = 2n + 1$
- $x$ is odd

> [!NOTE] **Remark 1**
>  In this case, we may prove both directions at once as we only use definitions and equalities, which are bidirectional, but proving each direction separately is clearer.

Proof. Let $x \in \mathbb{Z}$.
$$
\begin{aligned}
x \text { is odd } & \Leftrightarrow x=2 n+1 \text { for some } n \in \mathbb{Z} \\
& \Leftrightarrow x-1=2 n \text { for some } n \in \mathbb{Z} \\
& \Leftrightarrow x-1 \text { is even. }
\end{aligned}
$$

> [!NOTE] **Remark 2**
> Instead of proving $p \Rightarrow q$ directly, we prove its contrapositive, $\sim q \Rightarrow \sim p$, since a conditional is logically equivalent to its contrapositive.

**Proof by Contrapositive: To prove $p \Rightarrow q$, we prove $\sim q \Rightarrow \sim p$.**

> [!TIP] **Proposition 2**
> For every integer $x$, if $x^{2}$ is even, then $x$ is even.

**Contrapositive:** 
- For every integer $x$, if $x$ is not even, then $x^2$ is not even.

*Proof by Contraposition*
**Let $x \in \mathbb{Z}$ and suppose $x$ is not even:**
- then by proposition from last week, $x$ is odd.
	- $x = 2n+1$ for some $n \in \mathbb{Z}$
	- $x^2 = (2n+1)^2 = 4n^2+4n+1 = 2(2n^2+2n) + 1$ and $2n^2+2n \in \mathbb{Z}$
	- $x^2$ is odd, by definition.


> [!NOTE] **Remark 3**
> The contrapositive is easier to prove, because it is easier to infer information about $x^{2}$ from $x$ than to get information about $x$ from $x^{2}$.

> [!NOTE] **Remark 4**
> Let's rewrite the proposition using the fact that " $x$ is even" means " $2 \mid x$ "
- For every integer $x$, if $2|x^2$, then $2|x$

**We can generalize this to any prime $p$ :**
- For every integer $x$, and every prime $p$, if $p|x^2$, then $p|x$

Which is an immediate corollary of the following theorem:
( $\star$ ) For all integers $a, b$ and any prime $p$, if $p \mid a b$, then $p \mid a$ or $p \mid b$.
- take $a = b = x$

If we could use the theorem $(\star)$, then we didn't have to do the proof we did for Proposition 2 ! However, the proof of Proposition 2 is easier than the proof of $(\star)$, which we will do later.


> [!TIP] **Proposition 3**
> Let $a$ and $b$ be real numbers. If $a b=1$, then $a \leq 1$ or $b \leq 1$.

## Direct Proof. Let $a, b \in \mathbb{R}$.
- suppose $(a)(b) = 1$

**Case 1: Suppose $a \leq 1$. Then**
- we are done.

**Case 2: If $a>1$, then $b= \frac{1}{a} < 1$ and so $b \leq 1$.**
*Contrapositive*
- let $a, b \in \mathbb{R}$.
- if $a > 1 \land b > 1$ then $(a)(b) \neq 1$ 

Proof by Contraposition. Let $a, b \in \mathbb{R}$ and suppose $a>1$ and $b>1$.
- then $b > 1$ so $(a)(b) > a$ since $a > 1 ? 0$
- since $a > 1$, this implies $(a)(b)>1$
- so $(a)(b) \neq 1$

Then $ab > a(1) = a>1$ and so $a b \neq 1$.

Before we do another example, we give a direct proof a proposition we'll need.

---
> [!TIP] **Proposition 4**
> The product of an even integer and any integer is even. Proof. Let $x$ be an even integer and $y$ be an integer.
> 

Then $x=2 n$ for some integer $n$,
Therefore $xy=$ $(2n)y$
- $= 2(ny)$
	- $ny \in \mathbb{Z}$
- thus $xy$ is even, by definition
---
> [!TIP] **Proposition 5**
> If the product of two integers is odd, then the integers are not consecutive.

*Contrapositive*
- $x, y \in \mathbb{Z}$, if $x,y$ are consecutive, then $(x)(y)$ is even


Proof by Contraposition. Let $x$ and $x+1$ be two consecutive integers.

Case 1: If $x$ is even, then by Proposition 4, 
- $x(x+1)$ is even

Case 2: If $x$ is odd, then $x=2 n+1$ for some integer $n$, and so 
- $x+1= (2n+1)+1 = 2n+2 = 2(n+1)$
	- $n+1 \in \mathbb{Z}$
	- thus $x+1$ is even,
So, $x(x+1)$ is even, again by Proposition 4 .



> [!NOTE] **Remark 5**
> We have seen that to prove a biconditional $p \Leftrightarrow q$, we prove $p \Rightarrow q$ and $q \Rightarrow p$. Sometimes, one direction or the other may be easier to prove one direction using contrapositive. Since the contrapositive of the converse is the inverse, we have another option for how to prove the biconditional.

$$
\begin{aligned}
p \Leftrightarrow q & =p \Rightarrow q \wedge \quad q \Rightarrow p \\
& =p \Rightarrow q \wedge \sim p \Rightarrow \sim q
\end{aligned}
$$
$$
\text { To prove } p \Leftrightarrow q \text {, we may prove } p \Rightarrow q \text { and its inverse } \sim p \Rightarrow \sim q \text {. }
$$

---
> [!TIP] **Proposition 6**
> For every integer $x, x$ is odd if and only if $x^{2}-1$ is even.

## Proof:
$(\Rightarrow)$ First, we prove that if $x$ is odd, then $x^{2}-1$ is even.
**Let $x$ be an odd integer, then $x=2 n+1$ for some integer $n$.**
Therefore, $x^{2}-1=$
- $(2n+1)^2 - 1 = 4n^2+4n+1-1=4n^2=2(2n^2+2n)$
- $2n^2+2n \in \mathbb{Z}$
- And so $x^{2}-1$ is even.

$(\Leftarrow)$ We prove this direction by contraposition, which means we prove the inverse of what we just proved. We need to show that if $x$ is even (not odd), then $x^{2}-1$ is odd (not even).
Let $x$ be an even integer. Then $x=2 n$ for some integer $n$.
Therefore $x^{2}-1=$
- $(2n)^2-1 = 4n^2-1 = 4n^2-2+1 = 2(2n^2-1)+1$
- $2n^2-1 \in \mathbb{Z}$
- And so $x^{2}-1$ is odd.

> [!NOTE] **Remark 6**
> For this biconditional, it was easier to prove the inverse than the converse "if $x^{2}-1$ is even, then $x$ is odd" because it is easier to say something about $x^{2}-1$ if you know something about $x$ than it is the other way around.

# Exercises

1. Prove or disprove:
	For all integers $x$ and $y, x$ and $y$ are even if and only if $x+y$ is even.

2. Prove the following biconditionals:
	(a) An integer $x$ is even if and only if $x / 2$ is an integer.
	(b) An integer $x$ is odd if and only if $-x$ is odd.
	(c) An integer is odd if and only if it is a sum of two consecutive integers.
	(d) Let $a$ be an integer. Then $a^{2} \mid a$ if and only if $a=0,-1$, or 1 .

3. Prove the following proposition:
	Let $x \in \mathbb{Z}$ and $p, q$ be distinct primes. Then $p \mid x$ and $q \mid x$ if and only if $p q \mid x$.
	You may use the following theorem:
	*For every prime $p$ and all integers $a, b$, if $p \mid a b$, then $p \mid a$ or $p \mid b$.*

4. Prove the following statement:
	Let $x$ be an integer and $p$ a prime. Then $p \mid x$ if and only if $p \mid x^{2}$.
	You may use the following theorem:
	*For every prime $p$ and all integers $a, b$, if $p \mid a b$, then $p \mid a$ or $p \mid b$.*
5. Prove by contrapositive:
	(a) If $a-b$ is odd, then $a$ and $b$ have different parities.
	(b) For every integer $y$, if $y^{2}$ is odd, then $y$ is odd.
	(c) For every integer $y$, if $y^{3}$ is even, then $y$ is even.
	(d) If the product of two integers is even, then at least one of the factors is even.
	(e) If the product of two integers is odd, then the integers are not consecutive.
	(f) Let $n$ be an integer. If $4 \nmid n^{2}$, then $n$ is odd.
6. **For every integer $y, y$ is even if and only if $4 \mid\left(y^{2}+2 y\right)$.**
	- $a|b$ if $b = a(n)$, where $n \in \mathbb{Z}$
	**Case 1: Y is even**
	- $y = 2n$ for some $n \in \mathbb{Z}$
	- $y^2+2y = (2n)^2+2(2n)=4n^2+4n=4(n^2+n)$
		- $n^2+n \in \mathbb{Z}$
	**by contraposition**, prove $y$ is odd, and $4 ~|(y^2+2y)$
	- $y$ is odd, $y = 2n+1$ for some $n \in \mathbb{Z}$
	- $y^2+2y = (2n+1)^2+2(2n+1)$
	- $=4n^2 + 4n + 1 + 4n + 2$
	- $= 4n^2 + 8n +3$
	- $=4(n^2+2n) + 3$
		- $n^2+2n \in \mathbb{Z}$
	- 

Note: Prove one direction directly.
7. For all nonzero real numbers $x$ and $y,|x+y|=|x|+|y|$ if and only if $x$ and $y$ have the same sign.
Note: Prove one direction directly.
8. Let $x, y \in \mathbb{R}$. If $x y$ is irrational, then $x$ is irrational or $y$ is irrational.
9. Let $x$ be a real number. If $x$ is irrational, then $-x$ is irrational.


