# Definition 1.5.1

A set $A$ is a **subset** of a set $B$, written $A \subseteq B$, provided every
element of $A$ is also an element of $B$.

The set $B$ is sometimes called a **superset** of $A$.

We say $A$ is a **proper subset** of $B$, written $A \subset B$, provided
$A \subseteq B$ and $A \neq B$. In other words, if every element in $a$ is an
element in $B$, and there is at least one element in $B$ that is _not_ in $A$.

## Example 1.5.2

Let $A = \{x \in \mathbb{N}: x < 5\}$ and $B = \{x \in \mathbb{N}: x^2 < 10\}$.
Is $B \subseteq A$? Is $B$ a _proper_ subset of $A$?

**Solution** We are asking whether every natural number less than $5$ is also a
natural number whose square is less than $10$. Okay, we could just write out the
elements of the sets: $A = \{0, 1, 2, 3, 4\}$ and $B = \{0, 1, 2, 3\}$ (since
$3^2 = 9$ and $4^2 = 16$) . So $B \subseteq A$. But $B \neq A$, so in fact
$B \subset A$.
