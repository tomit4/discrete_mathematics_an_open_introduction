# 1.4.8 Additional Exercises

1.

Q: For a given predicate $P(x)$, you might believe that the statements
$\forall x P(x)$ or $\exists x P(x)$ are either true or false. How would you
decide if you were correct in each case? You have four choices: You could give
an example of an element $n$ in the domain for which $P(n)$ is true or for which
$P(n)$ is false, or you could argue that no matter what $n$ is, $P(n)$ is true
or is false.

(a) What would you need to do to prove $\forall x P(x)$ is true?

(b) What would you need to do to prove $\forall x P(x)$ is false?

\(c\) What would you need to do t prove $\exists x P(x)$ is true?

(d) What would you need to do to prove $\exists x P(x)$ is false?

A:

(a) What would you need to do to prove $\forall x P(x)$ is true?

I would need to prove that for any given $x$, $P(x)$ holds true.

(b) What would you need to do to prove $\forall x P(x)$ is false?

I would need to prove that there is at least one $x$ for which $P(x)$ is false.

\(c\) What would you need to do to prove $\exists x P(x)$ is true?

I would need to prove that there is at least one $x$ for which $P(x)$ holds
true.

(d) What would you need to do to prove $\exists x P(x)$ is false?

I would need to prove that for any given $x$, $P(x)$ is false.

2.

Q: Consider the statement, "For all integers $a$ and $b$, if $a + b$ is even,
then $a$ and $b$ are even."

(a) Write the contrapositive of the statement.

(b) Write the converse of the statement.

\(c\) Write the negation of the statement.

(d) Is the original statement true or false? Prove your answer.

(e) Is the contrapositive of the original statement true or false? Prove your
answer.

(f) Is the converse of the original statement true or false? Prove your answer.

(g) Is the negation of the original statement true or false? Prove your answer.

A:

Let's first establish what the original statement's antecedent and consequent
is:

"For all integers $a$ and $b$, if $a + b$ is even, then $a$ and $b$ are even."

$P(a, b)$ is "$a + b$ is even."

$Q(a, b)$ is "$a$ and $b$ are even."

$$ P(a, b) \to Q(a, b) $$

(a) Write the contrapositive of the statement.

$$ \neg Q(a, b) \to \neg P(a, b) $$

$\neg Q(a, b) \equiv \neg(E(a) \wedge E(b)) \equiv (\neg E(a) \vee \neg E(b))$
is "$a$ or $b$ are odd."

$\neg P(a, b)$ is $a + b$ is odd.

"For all integers $a$, and $b$, if $a$ or $b$ is odd, then $a + b$ is odd."

(b) Write the converse of the statement.

The converse is $Q(a, b) \to P(a, b)$.

"For all integers $a$ and $b$, if $a$ and $b$ are even, then $a + b$ is even."

\(c\) Write the negation of the statement.

The negation is $\neg(P(a, b) \to Q(a, b))$

$$ \neg(P \to Q) $$

$$ \neg(\neg P \vee Q) $$

$$ P \wedge \neg Q $$

$$ P(a, b) \wedge \neg Q(a, b) $$

"For all integers, $a$ and $b$, $a + b$ is even and either $a$ or $b$ are odd."

(d) Is the original statement true or false? Prove your answer.

"For all integers $a$ and $b$, if $a + b$ is even, then $a$ and $b$ are even."

Proof by Contradiction:

Let $a$ and $b$ be integers, and assume that $a + b$ is even and either $a$ or
$b$ are odd.

The sum of an even and an odd integer must be odd.

But then $a + b$ is both even and odd, a contradiction.

The original statement is false.

(e) Is the contrapositive of the original statement true or false? Prove your
answer.

"For all integers $a$, and $b$, if $a$ or $b$ is odd, then $a + b$ is odd."

Proof by Contradiction:

Let $a$ and $b$ be integers, assume either $a$ or $b$ is odd, and assume that
$a + b$ is even.

In the case that both $a$ and $b$ are odd, then $a + b$ is even (not a
contradiction).

But, in the case that $a$ is even and $b$ is odd, or in the case that $a$ is odd
and $b$ is even, then the sum $a + b$ must be odd.

But then $a + b$ is both even and odd, a contradiction.

This statement is false.

(f) Is the converse of the original statement true or false? Prove your answer.

Skipped (too much time)

(g) Is the negation of the original statement true or false? Prove your answer.

Skipped (too much time)

3.

Q: For each of the statements below, say what method of proof you should use to
prove them. Then say how the proof starts and how it ends. Bonus points for
filling in the middle.

(a) There are no integers $x$ and $y$ such that $x$ is a prime greater than 5
and $x = 6y + 3$.

(b) For all integers $n$, if $n$ is a multiple of 3, then $n$ can be written as
the sum of consecutive integers.

\(c\) For all integers $a$ and $b$, if $a^2 + b^2$ is odd, then $a$ or $b$ is
odd.

A:

(a) There are no integers $x$ and $y$ such that $x$ is a prime greater than 5
and $x = 6y + 3$.

Let $P(x)$ be "$x$ is prime", $Q(x)$ be "$x > 5$", $R(x,y)$ be "$x = 6y + 3$".

$$ \neg \exists x \exists y (P(x) \wedge Q(x) \wedge R(x,y)) $$

Method of Proof: Proof by Contradiction.

Start: Suppose there exist integers $x$ and $y$ such that $x$ is prime, $x > 5$,
and $x = 6y + 3$.

Middle: $x = 6y + 3 = 3(2y+1)$, so $x$ is divisible by 3. Since $x > 5$, we have
$x \neq 3$, so $x$ is composite, contradicting that $x$ is prime.

End: Therefore, no such integers $x$ and $y$ exist.

(b) For all integers $n$, if $n$ is a multiple of 3, then $n$ can be written as
the sum of consecutive integers.

$P(n)$ is "$n$ is a multiple of 3"

$Q(n)$ is "$n$ can be written as the sum of consecutive integers."

$$ \forall n (P(n) \to Q(n)) $$

Method of Proof: Direct Proof.

Start: Let $n$ be an integer, assume $n$ is a multiple of 3.

Middle: Say $n = 3k$ where $k$ is some integer. This means that we can sum
consecutive integers for $n$ as a sum centered around $k$:

$$ 3k = (k - 1) + k + (k + 1) $$

End: Therefore $n$ can be written as the sum of consecutive integers.

\(c\) For all integers $a$ and $b$, if $a^2 + b^2$ is odd, then $a$ or $b$ is
odd.

$P(a, b)$ is "a^2 + b^2 is odd"

$Q(a, b)$ is "$a$ is odd $\vee b$ is odd"

$$ \forall a \forall b (P(a, b) \to Q(a, b)) $$

Method of Proof: Contrapositive

Start: Let $a$ and $b$ be integers, and assume that both $a$ and $b$ are even.

Middle: An even number squared must be even, and the sum of two even numbers
also must be even.

End: Therefore $a^2 + b^2$ is even.

4.

Q: Consider the statement, "For all integers $n$, if $n$ is even then $8n$ is
even."

(a) Prove the statement. What sort of proof are you using?

(b) Is the converse true? Prove or disprove.

A:

(a) Prove the statement. What sort of proof are you using?

Let $P(n)$ be "$n$ is even."

Let $Q(n)$ be "$8n$ is even."

$$ \forall n (P(n) \to Q(n)) $$

Proof by Direct Proof:

Let $n$ be any integer, assume that $n$ is even.

Let $n = 2k$ where $k$ is any integer. We could then write:

$$ 8n = 8(2k) = 16k = 2(8k) $$

Any number that is a multiple of $2$ is even.

Therefore $8n$ is even.

(b) Is the converse true? Prove or disprove.

"For all integers $n$, if $8n$ is even, then $n$ is even."

$P(n)$ is "$8n$ is even."

$Q(n)$ is "$n$ is even."

$$ \forall n (P(n) \to Q(n)) $$

Proof by counterexample:

Let $n = 1$.

Then $8n = 8$, which is even.

But $n = 1$ is odd.

So we have an example where $8n$ is even but $n$ is odd.

Therefore the statement is false.
