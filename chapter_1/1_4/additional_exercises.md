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

5.

Q: The game TENZI comes with 40 six-sided dice (each numbered 1 to 6). Suppose
you roll all 40 dice.

(a) Prove that there will be at least seven dice that land on the same number.

(b) How many dice would you have to roll before you were guaranteed that some
four of them would all match or all be different? Prove your answer.

A:

(a) Prove that there will be at least seven dice that land on the same number.

Start:

Proof by Contradiction:

Start: Assume that seven of the dice do not land on the same number. This means
that each number on the die (from 1 to 6) appears at most 6 times among the 40
dice.

Middle: If each number from 1 to 6 appears at most 6 times, then the total
number of dice can be calculated as:

$$ 6(\text{appearances per number}) \times 6(\text{numbers}) = 36 $$

We have shown that if each number appears at most 6 times, then the maximum
number of dice is 36.

Since we are rolling 40 dice, which is more than 36, our initial assumption must
be false , which is a contradiction.

End: Therefore at least seven dice land on the same number.

(b) How many dice would you have to roll before you were guaranteed that some
four of them would all match or all be different? Prove your answer.

Proof by Contradiction:

Start: Assume that with 10 dice rolled, there are not four dice that all match
and there are not four dice that are all different.

Middle: Since there are not four matching dice, each number from 1 to 6 can
appear at most 3 times.

Also, since there are not four dice that are all different, there can be at most
3 different numbers appearing among the dice.

Therefore, the maximum number of dice possible is:

$$ 3(\text{copies of each number}) \times 3(\text{different numbers}) = 9 $$

But we rolled 10 dice, which is more than 9. This contradicts our assumption.

End: Therefore, if 10 dice are rolled, then there must be either four dice that
all match or four dice that are all different.

6.

Q: Prove that for all integers $n$, it is the case that $n$ is even if and only
if $3n$ is even. That is, prove both implications: If $n$ is even, then $3n$ is
even, and if $3n$ is even, then $n$ is even.

A:

Let $P(n)$ be "$n$ is even."

Let $Q(n)$ be "$3n$ is even."

We are trying to prove:

$$ \forall n (P(n) \leftrightarrow Q(n)) $$

Let's try to first prove the first implication:

"If $n$ is even, then $3n$ is even."

$$ \forall n (P(n) \to Q(n)) $$

Proof by Direct Proof:

Start: Assume that $n$ is even.

Middle: Let $n = 2k$ where $k$ is any integer, this means:

$$ 3n = 3(2k) = 6k = 2(3k) $$

Here we know that $3k$ can be even or odd, but any number multiplied by $2$ is
even.

End: Therefore $3n$ is even.

Now let's prove the other implication:

$$ \forall n (Q(n) \leftrightarrow P(n)) $$

"If $3n$ is even, then $n$ is even."

Proof by Contrapositive:

Start: Assume that $n$ is odd.

Middle: Let $n = 2k + 1$ where $k$ is any integer. Then:

$$ 3n = 3(2k + 1) = 6k + 3 = 2(3k + 1) + 1 $$

Since $3k + 1$ is an integer, $3n$ has the form of $2k + 1$, which is odd.

End: Therefore $3n$ is odd.

7.

Q: Prove that $\sqrt{3}$ is irrational.

A:

Proof by Contradiction:

Start: Assume that $\sqrt{3}$ is a rational number, which can be expressed with
integers $a$ and $b$. Let $a$ and $b$ be integers where $b \neq 0$, and
$\dfrac{a}{b}$ has $gcd(a, b) = 1$.

Middle:

This means we can write:

$$ \sqrt{3} = \frac{a}{b}  $$

If we then square both sides of this equation, we get:

$$ 3 = \frac{a^2}{b^2}  $$

$$ a^2 = 3b^2 $$

This implies that if $3$ divides $a$, then $3$ divides $b$.

So we can write $a = 3k$ for some integer $k$. This means that we can substitute
in $k$:

$$ a = 3k $$

$$ (3k)^2 = 3b^2 $$

$$ 9k^2  = 3b^2 $$

$$ 3k^2  = b^2 $$

So both $a$ and $b$ share a factor of 3. So the $gcd(a, b) \geq 3$.

But we assumed $gcd(a, b) = 1$. This is a contradiction.

End: Therefore, $\sqrt{3}$ is an irrational number.

8.

Q: Consider the statement, "For all integers $a$ and $b$, if $a$ is even and $b$
is a multiple of $3$, then $ab$ is a multiple of $6$."

(a) Prove the statement. What sort of proof are you using?

(b) State the converse. Is it true? Prove or disprove.

A:

(a) Prove the statement. What sort of proof are you using?

(b) State the converse. Is it true? Prove or disprove.

(a) We'll use a Proof by Direct Proof.

Proof by Direct Proof:

Let $a$ and $b$ be integers, where $a$ is even and $b$ is a multiple of $3$.

Since $a$ is even, we can express $a$ as $a = 2k$, where $k$ is any integer:

$$ a = 2k $$

And since $b$ is a multiple of $3$, we can express $b$ as $b = 3m$ where $m$ is
any integer.

$$ b = 3m $$

We can then express $ab$ as:

$$ ab = (2k)(3m) = 6km $$

Therefore, $ab$ is a multiple of $6$.

(b) State the converse. Is it true? Prove or disprove.

The converse statement is "For all integers $a$ and $b$, if $ab$ is a multiple
of $6$, then $a$ is even and $b$ is a multiple of $3$."

This statement is false.

Proof by Counterexample:

Consider $ab = 6$.

Let $a = 3$

$$ ab = 6 $$

$$ 3b = 6 $$

$$ b = 2 $$

So here, $a$ is not even, and $b$ is not a multiple of $3$, but $ab$ is a
multiple of $6$.

Therefore the statement is false.

9.

Q: Prove the statement, "For all integers $n$, if $5n$ is odd, then $n$ is odd."
Clearly state the style of proof you are using.

A:

Here instead we will prove the contrapositive statement:

"For all integers $n$, if $n$ is even, then $5n$ is even."

Proof by Contrapositive:

Let $n$ be an integer.

Let $n$ be $2k$ for some integer $k$. We can then write $5n$ as:

$$ 5n = 5(2k) = 10k = 2(5k) $$

So $5n$ is a multiple of $2.

Therefore $5n$ is even.

10.

Q: Prove the statement, "For all integers, $a$, $b$, and $c$, if
$a^2 + b^2 = c^2$, then $a$ or $b$ is even."

A:

Proof by Contrapositive:

Contrapositive statement:

"For all integers, $a$, $b$, and $c$, if $a$ and $b$ are odd, then
$a^2 + b^2 \neq c^2$"

Let $a$, $b$, and $c$ be integers, and assume that both $a$ and $b$ are odd.

Let $a = 2k + 1$ for any number $k$.

$$ a^2 = (2k + 1)^2 = 4k^2 + 4k + 1 = 2(2k^2 + 2k) + 1 $$

So here we have shown that $a^2$ is odd.

Let $b = 2m + 1$ for any number $m$.

$$ b^2 = (2m + 1)^2 = 4m^2 + 4m + 1 = 2(2m^2 + 2m) + 1 $$

So here we have shown that $b^2$ is odd.

And we know that any two odd numbers when added, their sum is an even number:

$$ \text{odd number} + \text{ odd number } = \text{ even number} $$

So, we can say that:

$$ a^2 + b^2 = \text{ even number} $$

And since $c^2$ must be an even number, then $c$ must also be an even number.

This shows that if $a$ and $b$ are both odd, then $c$ is even, and therefore
$a^2 + b^2 = c^2$ cannot contradict the claim that $a$ or $b$ is even. In other
words, either $a$ or $b$ must be even

Thus, the statement is true.

11.

Q: Suppose that you would like to prove the following implication:

    For all numbers, $n$, if $n$ is prime, then $n$ is solitary.

Write out the beginning and end of the argument if you were to prove the
statement,

(a) Directly

(b) By contrapositive

\(c\) By contradiction

You do not need to provide the middle parts of the proofs (since you do not know
what solitary means). However, make sure that you give the first few and last
lines of the proofs so that we can see the logical structure you would follow.

A:

(a) Directly

Beginning: Let $n$ be any integer where $n$ is prime.

End: Therefore $n$ is solitary.

(b) By contrapositive

Beginning: Let $n$ be any integer where $n$ is not solitary.

End: Therefore $n$ is not prime.

\(c\) By contradiction

Beginning: Let $n$ be any integer where $n$ is prime, assume that $n$ is not
solitary.

End: This is a contradiction.

12.

Q: Suppose you have a collection of rare 5-cent stamps and 8-cent stamps. You
desperately need to mail a letter and, having no other stamps available, decide
to dip into your collection. The question is, what amounts of postage can you
make?

(a) Prove that if you only use an even number of both types of stamps, the
amount of postage you make must be even.

(b) Suppose you made an even amount of postage. Prove that you used an even
number of at least one of the types of stamps.

\(c\) Suppose you made exactly 72 cents of postage. Prove that you used at least
6 of at least one type of stamp.

A:

(a) Prove that if you only use an even number of both types of stamps, the
amount of postage you make must be even.

Proof by Direct Proof:

Let $n$ be an even integer that represents the number of 5-cent stamps used, and
$m$ be an even integer that represents the number of 8-cent stamps used.

The sum for the amount of postage, $S$, then is:

$$ S = 5n + 8m $$

Let $n$ be $2k$ for any integer $k$, and $m$ be $2p$ for any integer $p$.

The sum for the amount of postage, $S$ then can be seen as:

$$ S = 5(2k) + 8(2p) = 10k + 16p = 2(5k + 8p) $$

Since $S$ is $2$ times an integer, it is even.

Therefore the amount of postage made must be even.

(b) Suppose you made an even amount of postage. Prove that you used an even
number of at least one of the types of stamps.

This is the converse of (a).

Proof by Contrapositive:

Let $n$ and $m$ both be odd integers

Let $S = 5n + 8m$ be the total postage.

Let $n$ be $2k + 1$ for any $k$ and $m$ be $2p + 1$ for any $p$.

Our sum becomes:

$$ S = 5(2k + 1) + 8(2p + 1) = 10k + 5 + 16p + 8 = 10k + 16p + 13 = 2(5k + 8p) + 13 $$

So $S$ is an odd number.

Therefore the amount of postage is not even.

\(c\) Suppose you made exactly 72 cents of postage. Prove that you used at least
6 of at least one type of stamp.

Proof by Contradiction:

Let $n$ be an integer that represents the number of 5-cent stamps used, and $m$
be an integer that represents the number of 8-cent stamps used. Assume that
$5n + 8m = 72$. Assume that $n < 6$ and $m < 6$.

If $n < 6$ and $m < 6$, this means that:

$$ n <= 5 $$

And

$$ m <= 5 $$

By setting $n$ and $m$ to their maximum values, we can evaluate $5n + 8n = 72$:

$$ 5(5) + 8(5) = 25 + 40 = 65 \neq 72  $$

But we assumed that $5n + 8m = 72$. This is a contradiction since $72 > 65$.

Therefore at least 6 of at least one type of stamp was used.

13.

Q: Prove: $x = y$ if and only if $xy = \dfrac{(x + y)^2}{4}$. Note, you will
need to prove two "directions" here, the "if" and the "only if" part.

A:

Let's start with the first "if" part:

Prove: $x = y$ if $xy = \dfrac{(x + y)^2}{4}$.

If $x = y$, then $xy = \dfrac{(x + y)^2}{4}$.

Proof by Direct Proof:

Let $x$ and $y$ be integers where $x = y$.

Since $x = y$, the following equation:

$$ xy = \frac{(x + y)^2}{4} $$

Can be written as:

$$ x^2 = \frac{(x + x)^2}{4} $$

Evaluation of the right-hand side of the equation shows:

$$ x^2 = \frac{(2x)^2}{4} $$

$$ x^2 = \frac{4x^2}{4} $$

$$ x^2 = x^2 $$

Therefore $xy = \dfrac{(x + y)^2}{4}$ when $x = y$.

And now let's prove the "only if" part:

Prove: $xy = \dfrac{(x + y)^2}{4}$ if $x = y$.

If $xy = \dfrac{(x + y)^2}{4}$, then $x = y$.

Proof by Direct Proof:

Let $x$ and $y$ be integers where $xy = \dfrac{(x + y)^2}{4}$.

Evaluating the equation:

$$ xy = \frac{(x + y)^2}{4} $$

$$ xy = \frac{(x + y)(x + y)}{4} $$

$$ xy = \frac{x^2 + 2xy + y^2}{4} $$

$$ 4xy = x^2 + 2xy + y^2 $$

$$ x^2 + 2xy + y^2 - 4xy = 0 $$

$$ x^2 - 2xy + y^2 = 0 $$

$$ (x - y)^2 = 0 $$

$$ x - y = 0 $$

$$ x = y $$

Therefore $x = y$ when $xy = \dfrac{(x + y)^2}{4}$.

14.

Q: Prove that $\log(7)$ is irrational.

A:

Proof by Contradiction:

Let $a$ and $b$ be integers where $b \neq 0$. Assume that
$\log(7) = \dfrac{a}{b}$.

Evaluating this equation:

$$ \log(7) = \frac{a}{b} $$

$$ 7 = 10^{\frac{a}{b}} $$

$$ 7 = \sqrt[b]{10^a}$$

$$ 7^b = 10^a $$

$7^b$ only has a prime factor of $7$, while $10^a$ has prime factors of $2$ and
$5$. But two integers with different prime factorizations cannot be equal.

Therefore $\log(7)$ is irrational.

15.

Q: Prove that there are no integer solutions to the equation $x^2 = 4y + 3$.

A:

Proof by Contradiction:

Let $x$ and $y$ be integers, and assume that $x^2 = 4y + 3$.

Since both $x$ and $y$ are integers, we can take $\mod 4$ of both sides and
evaluate:

$$ 4y \equiv 0 (\mod 4) $$

$$ 3 \equiv 3 (\mod 4) $$

$$ x^2 \equiv 3 $$

But we know that $x^2 \equiv (0 \vee 1) \mod 4$, so $x^2 \equiv 3$ is a
contradiction.

Therefore there are no integer solutions to the equation $x^2 = 4y + 3$.

16.

Q: Prove that every prime number greater than 3 is either one more or one less
than a multiple of 6.

A:

Proof by Direct Proof:

Let $p$ be some prime number greater where $p > 3$.

Consider $p = 6k + r$ where $k$ is any integer and $r$ represents some remainder
within the set $\{0, 1, 2, 3, 4, 5\}$.

$$ r \in \{0, 1, 2, 3, 4, 5\} $$

To be clear, $r$ represents all possible remaining values when an integer is
divided by 6.

Since $p$ is a prime number where $p > 3$, $p$ cannot be divisible by $2$ or
$3$.

Consider the following implications:

- $r = 0 \to p = 6k \to \text{ not prime}$

- $r = 2 \to p = 6k + 2  = 2(3k + 1) \to \text{ even } \to \text{ not prime}$

- $r = 3 \to p = 6k + 3 = 3(2k + 1) \to \text{ divisible by } 3 \to \text{ not prime}$

- $r = 4 \to p = 6k + 4  = 2(3k + 2) \to \text{ even } \to \text{ not prime}$

From the cases above, the only cases that do not make $p$ composite are $r = 1$
or $r = 5$.

This means that $p = 6k + 1$ is one more than a multiple of 6, and
$p = 6k + 5 = 6k - 1 + 6 = 6(k + 1) - 1$ is one less than a multiple of $6$.

Therefore every prime number greater than 3 is either one more or one less than
a multiple of 6.

17.

Q: Your "friend" has shown you a "proof" he wrote to show that $1 = 3$. Here is
the proof:

Proof: I claim that $1 = 3$. Of course we can do anything to one side of an
equation as long as we also do it to the other side. So subtract $2$ from both
sides. This gives $-1 = 1$. Now square both sides, to get $1 = 1$. And we all
agree this is true.

What is going on here? Is your friend's argument valid? Is the argument a proof
of the claim $1 = 3$? Carefully explain using what we know about logic.

A:

Our friend's argument is invalid. What is happening here is that our friend is
that our friend is making a mistake in their logic specifically when they square
both sides. They assume that if $a = b$, then $a^2 = b^2$, but the converse
statement of if $b^2 = a^2$, then $b = a$ does not hold (consider $(-1)^2$ as an
example).

18.

Q: A standard deck of 52 cards consists of 4 suits (hearts, diamonds, spades,
and clubs) each containing 13 different values (Ace, 2, 3, ..., 10, J, Q, K). If
you draw some number of cards at random, you might or might not have a pair (two
cards with the same value) or three cards all of the same suit. However, if you
draw enough cards, you will be guaranteed to have these. For each of the
following, find the smallest number of cards you would need to draw to be
guaranteed having the specified cards. Prove your answers.

(a) Three of a kind (for example, three 7's).

(b) A flush of five cards (for example, five hearts).

\(c\) Three cards that are either all the same suit or all different suits.

A:

(a) Three of a kind (for example, three 7's).

Proof by Direct Proof:

Let 13 be the number of different values in a standard deck of 52 cards
consisting of 4 suits.

Consider we try and avoid drawing three of a kind for as long as possible. This
means we would draw at most 2 cards into each of the 13 values. This gives a
maximum of:

$$ 2 \times 13 = 26 $$

Here we would have 26 cards without having 3 cards of the same values.

Consider what would happen if we drew one more card.

$$ 26 + 1 = 27 $$

By the Pigeonhole Principle, when we distribute 27 cards among 13 ranks, at
least one rank must contain at least 3 cards:

$$ \left\lceil\frac{27}{13}\right\rceil \geq 3 $$

Therefore, drawing 27 cards would be needed to guarantee having three of a kind.

(b) A flush of five cards (for example, five hearts).

Proof by Direct Proof:

Let 4 be the number of different suits in a standard deck of 52 cards.

Consider we try and avoid drawing 5 cards of the same suit for as long as
possible. This means we would draw at most 4 cards into each of the 4 suits.
This gives a maximum of:

$$ 4 \times 4 = 16 $$

Here we would have 16 cards without having 5 cards of the same suit.

Now consider what would happen if we drew one more card:

$$ 16 + 1 = 17 $$

By the Pigeonhole Principle, when we distribute 17 cards among 4 suits, at least
one suit must contain at least 5 cards:

$$ \left\lceil\frac{17}{4}\right\rceil \geq 5 $$

Therefore, drawing 17 cards would be needed to guarantee having a flush of five
cards.

\(c\) Three cards that are either all the same suit or all different suits.

Proof by Direct Proof:

First, 4 cards are not sufficient: choose 2 hearts and 2 spades. Then no suit
has 3 cards, and only two suits appear, so it is impossible to have 3 cards all
of different suits. Hence, 4 does not guarantee the condition.

Now consider any set of 5 cards. If any suit appears at least 3 times, we are
done. Otherwise, each suit appears at most twice. Since $5 > 2 \cdot 2 = 4$, at
least three different suits must appear among the five cards, so we can choose
one card from each of three suits to obtain three cards all of different suits.

Thus, every set of 5 cards satisfies the condition, and 5 is minimal.

19.

Q: Suppose you are at a party with 19 of your closest friends (so, including
you, there are 20 people there). Explain why there must be at least two people
at the party who are friends with the same number of people at the party. Assume
friendship is always reciprocated.

A:

Proof by Direct Proof:

Let there be 20 people at the party. For each person, let $d$ be the number of
friends they have at the party. Then $d \in \{0, 1, 2, \dots, 19\}$.

Consider that it is impossible for both a person with 19 friends and a person
with 0 friends to exist simultaneously, since friendship is reciprocal.
Therefore, at most 19 distinct values of $d$ can occur among the 20 people.

By the Pigeonhole Principle, two people must have the same value of $d$.

Therefore, at least two people have the same number of friends at the party.

20.

Q: Your friend has given you his list of 115 best Doctor Who episodes (in order
of greatness). It turns out that you have seen 60 of them. Prove that there are
at least two episodes you have seen that are exactly four episodes apart on your
friend's list.

A:

Proof by Direct Proof:

Label the episodes $1, 2, \dots, 115$, Let $S$ be the set of indices of the 60
episodes you have seen.

Partition the 115 indices into 4 residue classes modulo 4:

$$ \{1, 5, 9, \dots\}, \quad \{2, 6, 10, \dots\}, \quad \{3, 7, 11, \dots\}, \quad \{4, 8, 12, \dots\} $$

These are 4 disjoint classes.

Since there are 60 indices in $s$ and only 4 classes, by the Pigeonhole
Principle, one of these classes contains at least two elements of $S$.

So there exists two seen episodes whose indices differ by a multiple of 4.

Now, within a single residue class, the elements occur in increasing order
spaced exactly by 4, so the closest such pair must differ by exactly 4.

Therefore, there exists two episodes you have seen that are exactly four
episodes apart on the list.
