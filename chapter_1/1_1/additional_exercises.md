# 1.1.6 Additional Exercises

1.

Q: Suppose $P$ and $Q$ are the statements: $P$: Jack passed math. $Q$: Jill
passed math.

(a) Translate "Jack and Jill both passed math" into symbols.

(b) Translate "If Jack passed math, then Jill did not" into symbols.

\(c\) Translate "$P \vee Q$" into English

(d) Translate "$\neg(P \wedge Q) \to Q$" into English.

(e) Suppose you know that if Jack passed math, then so did Jill. What can you
conclude if you know that:

i. Jill passed math?

ii. Jill did not pass math?

A:

(a) Translate "Jack and Jill both passed math" into symbols.

$$ P \wedge Q $$

(b) Translate "If Jack passed math, then Jill did not" into symbols.

$$ P \to \neg Q $$

\(c\) Translate "$P \vee Q$" into English

"Either Jack passed math or Jill passed math or they both passed math."

(d) Translate "$\neg(P \wedge Q) \to Q$" into English.

"If it is true that Jack did not pass math or Jill did not pass math or both did
not pass math, then Jill passed math."

(e) Suppose you know that if Jack passed math, then so did Jill. What can you
conclude if you know that:

i. Jill passed math?

$$ P \to Q $$

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

While it is true that Jack passed math:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |

It is also possible that Jack did not pass math:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | T   | T         |

Therefore we can say that while it is true that "If Jack passed math, then Jill
passed math." And it is also true that "Jill passed math.", we cannot know if
"Jack passed math" is a true or false statement.

ii. Jill did not pass math?

$$ P \to Q $$

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | F   | F         |
| F   | F   | T         |

So given our first assumption, which is that if "Jack passed math, then Jill
passed math", $P \to Q$, is a true statement. We are also told by part ii that
Jill did not pass math. Given this, and given that we know that $P \to Q$ is
true, we can only therefore take the last row:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | F   | T         |

So we know that Jack did not pass math.

2.

Q: Translate into symbols. Use $E(x)$ for "$x$ is even" and $O(x)$ for "$x$ is
odd."

(a) No number is both even and odd.

(b) One more than any even number is an odd number.

\(c\) There is a prime number that is even.

(d) Between any two numbers there is a third number.

(e) There is no number between a number and one more than that number.

A:

(a) No number is both even and odd.

$$ \forall x \neg (E(x) \wedge O(x)) $$

Also:

$$ \neg \exists x (E(x) \wedge O(x)) $$

(b) One more than any even number is an odd number.

$$ \forall x (E(x) \to O(x + 1)) $$

\(c\) There is a prime number that is even.

Say that $P(x)$ symbolizes "$x$ is prime." then:

$$ \exists x (P(x) \wedge E(x)) $$

(d) Between any two numbers there is a third number.

This one goes outside the scope of the section a bit, but you can say:

$$ \forall x \forall z \left(x < z \to \exists y(x < y < z)\right) $$

(e) There is no number between a number and one more than that number.

$$ \forall x \neg \exists y (x < y < x + 1) $$

3.

Q: For each of the statements below, give a domain of discourse for which the
statement is true, and a domain for which the statement is false.

(a) $\forall x \exists y \left(y^2 = x\right)$.

(b) $\forall x \forall y \left(x < y \to \exists z(x < z < y)\right)$.

\(c\) $\exists x \forall y \forall z(y < z \to y \leq x \leq z)$.

A:

(a) $\forall x \exists y \left(y^2 = x\right)$.

The domain of discourse for the statement is true for all real numbers greater
than or equal to $0$.

$$ \text{DOMAIN WHERE TRUE: } \forall x \exists y \left(y^2 = x\right), x \in \mathbb{R_{\geq 0}} $$

The domain of discourse for this statement is false for all real numbers (or
integers) less than $0$

$$ \text{DOMAIN WHERE FALSE: } \forall x \exists y \left(y^2 = x\right), x \in \mathbb{R_{<0}} $$

(b) $\forall x \forall y \left(x < y \to \exists z(x < z < y)\right)$.

This is true for the domain of all real numbers:

$$ x, y, z \in \mathbb{R} $$

This is false for the domain of all whole integers, since there is no number
between, say $2$ and $3$ in $\mathbb{Z}$:

$$ x, y, z \in \mathbb{Z} $$

\(c\) $\exists x \forall y \forall z(y < z \to y \leq x \leq z)$.

This statement is true in any domain with at most one element, and false in any
ordered set with at least two distinct elements.

Examples:

True in: $\{0\}$ False in: $\mathbb{Z}, \mathbb{R}$
