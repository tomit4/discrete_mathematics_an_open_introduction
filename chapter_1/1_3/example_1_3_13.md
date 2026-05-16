# Example 1.3.13

Can you switch the order of quantifiers? For example, consider the two
statements:

$$ \forall x \exists y P(x, y) \quad \text{ and } \quad \exists y \forall x P(x, y) $$

Are these logically equivalent?

**Solution**.

These statements are NOT logically equivalent. To see this, we should provide an
interpretation of the predicate $P(x, y)$ which makes one of the statements true
and the other false.

Let $P(x, y)$ be the predicate $x < y$. It is true, in the natural numbers, that
for all $x$ there is some $y$ greater than that $x$ (since there are infinitely
many numbers). However, there is no natural number $y$ which is greater than
every number $x$. Thus it is possible for $\forall x \exists y P(x, y)$ to be
true while $\exists y \forall x P(x, y)$ is false.

We cannot do the reverse of this though. If there is some $y$ for which every
$x$ satisfies $P(x, y)$, then certainly for every $x$ there is some $y$ which
satisfies $P(x, y)$. The first is saying we can find one $y$ that works for
every $x$. The second allows different $y$'s to work for different $x$'s, but
nothing is preventing us from using the same $y$ that works for every $x$. In
other words, while we don't have logical equivalence between the two statements,
we do have a valid deduction rule:

$$
\exists y \forall x P(x, y) \\
\overline{\therefore \forall x \exists y P(x, y)}
$$

Put yet another way, this says that the single statement

$$ \exists y \forall x P(x, y) \to \forall x \exists y P(x, y) $$

is always true; it is a law of logic.
