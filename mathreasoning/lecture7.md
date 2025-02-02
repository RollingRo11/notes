# Lecture 7: 1/30/2025

Proof by Contradiction: Assume the statement is false, then deduce a logical impossibility.

> [!TIP] **Proposition 1**
> *There is no largest integer.*

*Proof.*




> [!NOTE] **Remark 1**
> In a proof by contradiction, we assume that the assertion is false, or its negation is true. We then proceed until we reach a contradiction, that is, something false or absurd. This must mean that the negation is false, and the assertion is true. This argument is reductio ad absurdum in Latin: reduction to absurdity.

> [!NOTE] **Remark 2**
> If we start a proof assuming that the assertion is false, then it is clear that we are doing a proof by contradiction, we may omit the last sentence in the above proof (blue). Some people omit more, ending the above proof with, ". . y y is larger than $x$, contradiction!" (or $\rightarrow \leftarrow$, which denotes contradiction). For a beginner, it is a good idea to state explicitly what the contradiction is.

- It is possible that a direct proof and a proof by contradiction are equally good.

> [!TIP] **Proposition 2**
> Consecutive integers cannot be both even.

*Direct Proof*

*Proof by Contradiction.*

- Sometimes a proof by contradiction is clearly the way to go!

> [!TIP] **Proposition 3**
> $\sqrt{2}$ is irrational.


Proof. Suppose $\sqrt{2} \in \mathbb{Q}$. Then $\sqrt{2}$ can be written as an irreducible fraction of integers, i.e.

$$
\sqrt{2}=\frac{m}{n}
$$

where $m$ and $n$ do not have a common factor/divisor (other than 1 and -1 ).

> [!TIP] **Proposition 4**.
> There are infinitely many primes.

*Proof*.

We will assume the Fundamental Theorem of Arithmetic ${ }^{1}$ (FTA) is true.

Fundamental Theorem of Arithmetic: Any integer $n \geq 2$ has a prime factor.

Suppose there are finitely many primes, call them $p_{1}, p_{2}, \ldots, p_{t}$. Consider $n=p_{1} p_{2} p_{3} \cdots p_{t}+1$. Then...

> [!NOTE] **Remark 3**.
> Theorems often come in the form $p \Rightarrow q$. To prove $p \Rightarrow q$ by contradiction, we suppose $\sim(p \Rightarrow q)$ and come to an absurd conclusion. Since $\sim(p \Rightarrow q)=p \wedge \sim q$, we can prove $p \Rightarrow q$ by assuming that $p \wedge \sim q$ and proceeding with logic until we arrive at a contradiction. Many conditional statements $p \Rightarrow q$ can be proved both ways: by contrapositive or by contradiction. The proofs are NOT exactly the same.

- Proof by contrapositive shows that $\sim q \Rightarrow \sim p$ is true
- Proof by contradiction shows that the negation of $\sim(p \Rightarrow q)$, that is, $p \wedge \sim q$, is false.

Proof of $p \Rightarrow q$ by Contradiction: Suppose $p \wedge \sim q$ and deduce a logical impossibility.

Last time we gave a proof of the following proposition by contraposition. Now we give a proof by contradiction.

Proposition 5. Let $a$ and $b$ be real numbers. If $a b=1$, then $a \leq 1$ or $b \leq 1$.

Proof by Contradiction.

Remark 4. Recall the definition of subset: set $A$ is a subset of set $B$ iff every element of $A$ is an element of $B$. This is equivalent to: "If $x \in A$, then $x \in B$."

To prove $A \subseteq B$ : $\quad$ Let $x \in A$. Then show that $x \in B$.

Proposition 6. If $A$ is the set of multiples of 4 and $B$ is the set of even integers, then $A \subseteq B$.
$A=$
$B=$

Proof.

> [!NOTE] **Remark 5**.
> Recall that $A=B$ iff $A$ and $B$ contain exactly the same elements, i.e. every element of $A$ is also in $B$, and vice versa, which means exactly that $A \subseteq B$ and $B \subseteq A$, so...

To prove $A=B$ : $\quad$ Show that $A \subseteq B$ and that $B \subseteq A$.

> [!TIP] Proposition 7
> Let $S=\{2 m-3 n: m, n \in \mathbb{Z}\}$, then $S=\mathbb{Z}$.


Proof. Let $x \in S$. Then...

Next, let $x \in \mathbb{Z}$. Then...

Theorem 1 (Laws for Sets).

$$
\begin{aligned}
A \cap B & =B \cap A \\
(A \cap B) \cap C & =A \cap(B \cap C) \\
A \cap(B \cup C) & =(A \cap B) \cup(A \cap C) \\
A \cap A & =A \\
\overline{A \cap B} & =\bar{A} \cup \bar{B} \\
A \cap B \subseteq A \quad A & \cap B \subseteq B
\end{aligned}
$$

$$
\begin{aligned}
A \cup B & =B \cup A \\
(A \cup B) \cup C & =A \cup(B \cup C) \\
A \cup(B \cap C) & =(A \cup B) \cap(A \cup C) \\
A \cup A & =A \\
\overline{A \cup B} & =\bar{A} \cap \bar{B} \\
B \subseteq A \cup B \quad A & \cap B \subseteq A \cup B
\end{aligned}
$$

$A \subseteq A \cup B$
(Commutative)
(Associative)
(Distributive)
(Idempotent)
(De Morgan)
(Int/Union Subsets)

Remark 6. We will use the above laws without further proof as they follow directly from the corresponding logical equivalences in Lessons 3. For example, consider the commutative law:

We have $A \cap B=B \cap A$ since " $x \in A$ and $x \in B$ " if and only if " $x \in B$ and $x \in A$ ". $\quad(p \wedge q=q \wedge p)$

Remark 7. A Venn diagram can be used to effectively illustrate and understand a set equivalence, although Venn diagrams are not accepted as a formal proof by most, including us.

We give a Venn diagram illustration of the De Morgan's Law $\overline{A \cap B}=\bar{A} \cup \bar{B}$.
![](https://cdn.mathpix.com/cropped/2025_02_02_f1875d0b3241d6397686g-6.jpg?height=222&width=1104&top_left_y=1380&top_left_x=505)

We give a Venn diagram illustration of the De Morgan's Law $\overline{A \cup B}=\bar{A} \cap \bar{B}$.
![](https://cdn.mathpix.com/cropped/2025_02_02_f1875d0b3241d6397686g-6.jpg?height=221&width=1107&top_left_y=1784&top_left_x=505)

Proposition 8. Let $A$ and $B$ be sets. If $A \subseteq B$, then $\bar{B} \subseteq \bar{A}$.
Proof.

Proposition 9. Let $A$ and $B$ be sets. Then $A \cap B=A$ if and only if $A \subseteq B$.
Proof.
$(\Rightarrow)$
$(\Leftarrow)$

Proposition 10. Let $A, B$, and $C$ be sets. If $A \subseteq B$, then $A \times C \subseteq B \times C$.
Proof.

## Exercises for Proof by Contradiction

## Prove by contradiction:

1. There is no largest even integer.
2. There is no largest irrational number.
3. There are no integers $a$ and $b$ such that $25 a-15 b=3$.
4. There are no integers $x$ and $y$ such that $4 x^{2}-y^{2}=1$. Hint: Factor $4 x^{2}-y^{2}$.
5. The only even prime is 2 .
6. If the sum of two primes is prime, then one of the primes must be 2. Note: You may use the proposition in \#5.
7. The sum of a rational and irrational number is irrational.
8. For all prime $p, \sqrt{p}$ is irrational. Note: You may use the following: For every prime $p$ and all integers $a, b$, if $p \mid a b$, then $p \mid a$ or $p \mid b$.
9. $\sqrt[3]{2}$ is irrational.
10. Let $S$ be a subset of $\mathbb{R}$ which is bounded below (see Exercise 4 in Lesson 5). We have an axiom called the Well-Ordering Principle (WOP):

- Any nonempty subset of $\mathbb{Z}$ bounded below has a least element.

This axiom is intuitive and "self-evident", and we accept it without proof.
(a) Find the least element of $A=\{x \in \mathbb{Z}: x \geq 0\}$ and $B=\{x \in \mathbb{Z}: x>0\}$.
(b) Prove that the positive real numbers $\mathbb{R}^{+}=(0, \infty)$ is bounded below, find the greatest lower bound (glb).
(c) Prove by contradiction that $\mathbb{R}^{+}$has no smallest element.

For the following propositions, give a direct proof and a proof by contradiction.
11. If $a$ and $b$ are real numbers and $a b=0$, then $a=0$ or $b=0$.
12. If $a$ and $b$ are real numbers and $a+b=0$, then $a \leq 0$ or $b \leq 0$.
13. The product of two consecutive integers is non-negative.
14. (Optional) Prove by contradiction that it is not possible to cover a $6 \times 6$ chessboard using $1 \times 4$ pieces. Hint: Number the board as follows:
$\begin{array}{lllll}1 & 2 & 3 & 4 & 2\end{array}$
234123
$\begin{array}{llllll}3 & 4 & 1 & 2 & 3 & 4\end{array}$
$\begin{array}{lllll}4 & 1 & 2 & 4\end{array}$
$\begin{array}{llll}1 & 2 & 312\end{array}$
234123
Every $1 \times 4$ piece covers " 4 " exactly once; how many 4's are on the board?

## Exercises for Set Proofs

1. Prove the following proposition: Suppose $a, b \in \mathbb{Z}, A=\{x \in \mathbb{Z}: a \mid x\}$ and $B=\{x \in \mathbb{Z}: b \mid x\}$, then $A \subseteq B$ if and only if $b \mid a$.
2. Let $A=\{x \in \mathbb{Z}: 6 \mid x\}$ and $B=\{15 n-9 m: n, m \in \mathbb{Z}\}$. Prove that $A \subseteq B$ but $A \neq B$.
3. Let $A, B, C$ denote sets. Consider the following set relation.

$$
(A \backslash B) \backslash C=A \backslash(B \cup C)
$$

Use a Venn diagram illustration to show the above equivalence.
4. Let $A$ and $B$ be subsets of integers, and we define:

$$
A+B=\{a+b: a \in A, b \in B\}
$$

Prove that if $A$ is the set of negative integers and $B$ is the set of even integers, then $A+B=\mathbb{Z}$.
5. Let $A$ and $B$ be any subsets of integers and define:

$$
A B=\{a b: a \in A, b \in B\}
$$

Let $A$ be the set of even integers. Prove that if $A B=A$, then $1 \in B$ or $-1 \in B$.
Hint: You may start with $2 \in A B$, explain why, and continue from there.
Let $A, B, C$ be sets. Prove or disprove:
6. If $A \subseteq B$ then $A \cup B=B$.
7. If $A \backslash B=A$, then $A$ and $B$ are disjoint.
8. If $A \subseteq B$ and $B \subseteq C$, then $A \subseteq C$.
9. If $A \subseteq C$ and $B \subseteq C$, then
(a) $A \cap B \subseteq C$
(b) $A \cup B \subseteq C$
10. If $A \backslash B=\emptyset$, then $B \backslash A=\emptyset$.
11. $A \backslash(B \cup C)=(A \backslash B) \cup(A \backslash C)$
12. $B=\bar{A}$ if and only if $A$ and $B$ are disjoint.
13. If $A \backslash B=B \backslash A$, then $A=B$.
14. $A=B$ if and only if $A \cap B=A \cup B$.
15. $A \backslash B$ and $B \backslash A$ are disjoint.
16. $A \backslash B=\emptyset$ if and only if $A \subseteq B$.




