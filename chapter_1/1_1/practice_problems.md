1.

Q: For each sentence below, decide whether it is an atomic statement, a
molecular statement, or not a statement at all.

(a) Some say the end is near, and some say we'll see Armageddon soon.

(b) Mom's coming 'round to put it back the way it ought to be.

(c) Learn to swim.

A:

(a) This is moleculr statement, two predicates are asserted, one is that "Some
say the end is near" and the other is "some say we'll see armageddon".

If we say $P(x)$ is "some say the end is near", and $Q(x)$ is "some say we'll
see Armageddon soon", we can write this as:

$$ \exists x \left(P(x) \wedge Q(x)\right) $$

(b) This can be reversed as "if there's a way it ought to be, then Mom is coming
'round to put it back."

If we say that $x$ is "it", and $P(x)$ is "the way it ought to be", and $Q(x)$
is "Mom is coming round to put it back," then we can write this as:

$$ P(x) \to Q(x) $$

This is an atomic statement, as both $P(x)$ and $Q(x)$ cannot be divided into
smaller elements.

(c) Learn to swim.

This is not a statement, there is no assertion made.

---

2.

Q: Classify each of the sentences below as an atomic statement, a molecular
statement, or not a statement at all. If the statement is molecular, say what
kind it is (conjunction, disjunction, conditional, biconditional, negation).

(a) Everybody can be fooled sometimes.

This is molecular due to the "sometimes" statement.

If we say that $x$ is somebody, and $y$ is some point in time. And if we say
that $P(x)$ is some situation somebody is in, and $Q(y)$ is "being fooled at
some point in time", then we can express this as:

$$ \forall x \exists y\left(P(x) \to Q(y)\right) $$

And this is a conjunction.

W: atomic

(b) Every natural number greater than 1 is either prime or composite.

This is also molecular. Let's break this down. If we say that $x$ is some
natural number, and $P(x)$ is "$x$ is prime", and $Q(x)$ is "$x$ is composite",
then we can say that:

$$ \forall (x > 1) \in \mathbb{N} \left(P(x) \vee Q(x)\right) $$

This is an disjunction.

(c) Go to your room!

This is not a statement as no assertion is made.

(d) The Broncos will win the Super Bowl, or I'll eat my hat.

This is an atomic statement. If we say that $P$ is "The Broncos will win the
Super Bowl", and we say that $Q$ is "I'll eat my hat". Then we can express this
as:

$$ P \vee Q $$

W: this is molecular.

(e) This shirt is not black.

Here an assertion is made, but no conclusion is drawn, so this is not a
statement. If we say that $P$ is "This shirt is black", then we are only left
with:

$$ \neg P $$

And there is no conclusion $Q$ to be drawn.

This is not a statement.

W: this is a statement. $\neg P$ is a statement.

---

3.

Q: Determine whether each molecular statement below is true or false, or whether
it is impossible to determine. Assume you do not know what my favorite number is
(but you do know which numbers are prime).

(a) If 4 is my favorite number, then 4 + 1 is my favorite number.

(b) 8 is my favorite number, and 3 is not prime.

(c) 4 is my favorite number, or 4 is prime.

(d) If 4 is prime then 2 $\cdot$ 4 is prime.

(e) If 3 is prime, then 3 is my favorite number.

(f) 8 is my favorite number, and 4 is not prime.

A:

(a) If 4 is my favorite number, then 4 + 1 is my favorite number.

We can not determine this as we do not know if $4$ is my favorite number.

$$ P(4) \to P(5) $$

(b) 8 is my favorite number, and 3 is not prime.

False, although we are saying that $P(8)$ is true, our original statement says
we cannot know that, and we say that Q(3) is "3 is prime", then we can say

$$ P(8) \wedge \neg Q(3) $$

Which is a false statement as, again $P(8)$ is unknown and $\neg Q(3)$ is false.

(c) 4 is my favorite number, or 4 is prime.

This is a false statement, we are saying that $P(4)$ is true, but we cannot know
that (like in problem 3). And we're saying that $Q(4)$ as being "4 is prime".
While $Q(4)$ is not true, $P(4)$ is unknown, and this implies the following:

$$ P(4) \vee Q(4) $$

Which is a false statement since $P(4)$ is unknown and $Q(4)$ is false.

(d) If 4 is prime then 2 $\cdot$ 4 is prime.

This is a true statement. If we say that $P(x)$ is true if 4 is prime, then we
can say that $Q(x)$ is true if 2 $\cdot$ 4 is prime.

$$ P(x) \to Q(x) $$

Since $P(x)$ and $Q(x)$ is false, this means that $P(x) \to Q(x)$ is true (see
truth tables).

(e) If 3 is prime, then 3 is my favorite number.

This is a not possible to determine. We say that $P$ is "3 is prime", which is
true, but then we say that $Q$ is "3 is my favorite number", it follows that:

$$ P \to Q $$

Since $P$ is true, but $Q$ is unknown, we cannot determine the validity of this
statement

(f) 8 is my favorite number, and 4 is not prime.

We can say that this is not possible to determine. We can declare $P(8)$ is "8
is my favorite number" as true, but we cannot know that. Also "4 is prime" is
expressed as $Q(4)$, but is false so therefore:

$$ P(8) \wedge \neg Q(4) $$

Is unkonwn because $P(8)$ is unknown and $\neq Q(4)$ is true, but both must be
true for this statement to be true, and so therefore this statement is not
possible to determine.

4.

Q: Let $P(x, y)$ be the predicate, "person $x$ can be fooled at time $y$."

Match each statement with its representation in symbols.

|                                                  |                               |
| ------------------------------------------------ | ----------------------------- |
| It is always true that some people can be fooled | $\exists x \forall y P(x, y)$ |
| Sometimes everyone can be fooled.                | $\forall x \exists y P(x, y)$ |
| Everyone can be fooled sometimes.                | $\forall y \exists x P(x, y)$ |
| Some people can be fooled all of the time.       | $\exists y\forall x P(x, y)$  |

A:

|                                                  |                               |
| ------------------------------------------------ | ----------------------------- |
| It is always true that some people can be fooled | $\forall y \exists x P(x, y)$ |
| Sometimes everyone can be fooled.                | $\exists y \forall x P(x, y)$ |
| Everyone can be fooled sometimes.                | $\forall x \exists y P(x, y)$ |
| Some people can be fooled all of the time.       | $\exists x\forall y P(x, y)$  |

5.

Q: Your friend believes that you cannot fool everyone at the same time. What is
another way of saying this, and how would you write that in symbols (using
$P(x, y)$ to say you can fool $x$ at time $y$).

A. Someone is never fooled. $\exists x \forall y \neg P(x, y)$

B. Everyone is never fooled. $\forall x \forall y \neg P(x, y)$

C. Someone is not fooled sometimes. $\exists x \exists y \neg P (x, y)$

D. Everyone is not fooled sometimes. $\forall x \exists y \neg P (x, y)$

A:

I'd say D is correct.

6.

Q: Regardless of your beliefs of how many people can be fooled at various times,
what could you conclude if we reinterpret $P(x, y)$ to mean $x < y$ and only
quantify over the natural numbers (so $\forall x$ means "For all natural
numbers," and $\exists x$ means "There exists a natural number")? Select all of
the following that apply.

A. $\forall x \exists y P(x, y)$ is true.

B. $\exists x \forall y P(x, y)$ is true.

C. $\forall y \exists x P(x, y)$ is true.

D. $\exists y \forall x P(x, y)$ is true.

E. No matter what $P(x, y)$ means, we can conclude that
$\forall x \exists y P(x, y)$ and $\exists y \forall x$ are NOT _logically
equivalent_

A:

A. This is true. We interpret this as "For all numbers for $x$, there exists
some number, $y$ where $x < y$". If $x \in \mathbb{N}$, then we know that this
is the same meaning as $x \in [0, \infty)$. We're essentially saying that every
possible value for $x$, there exists some value for $y$ that must be greater
than $x$. That's true.

B. This is false. "There exists some number, $x$, for all possible numbers for
$y$ where $x < y$". This means that some value of $x$ will always be less than
every possible $y$, that cannot be true.

C. This is true. "For all possible values for $y$, there exists some value $x$
where $x < y$." This is saying that for any given value for $y$, we can always
find at least one value for $x$ where $x < y$.

D. This is false. "There exists some value for $y$ such that for all possible
values of $x$, $x < y$." This would mean there is a natural number $y$ that is
greater than every natural number $x$, but this is impossible because for any
$y$, we can choose $x = y$, which makes $x < y$ false.

E. This is true. The statements $\forall x \exists y\, P(x,y)$ and
$\exists y \forall x\, P(x,y)$ are not logically equivalent.

The first means: for every value of $x$, there exists some value of $y$ such
that $x < y$. This is true for natural numbers since we can always choose a
larger number.

The second means: there exists some value of $y$ such that for all values of
$x$, $x < y$. This is false, because for any choice of $y$, we can take $x = y$,
which makes $x < y$ false.

The two statements, in essence, logically contradict each other.

7.

Q: Let $P(x)$ be the predicate, "$17x + 1$ is even."

(a) Is $P(15)$ true or false?

(b) What, if anything, can yhou conclude about $\exists x P(x)$ from the truth
value of $P(15)$?

(c) What, if anything, can you conclude about $\forall x P(x)$ from the truth
value of $P(15)$?

A:

(a) Yes, simple arithmetic shows that if the predicate states:

$$ P(x) = (17x + 1) \mod 2 = 0 $$

Then:

$$ P(15) = (17(15) + 1) = 256 \mod 2 = 0 $$

Therefore the statement $P(15)$ is true.

(b)

We can conclude that this statement, $\exists x P(x)$ is true. This is saying
"There exists some value for $x$ where $17x + 1$ is even." This is definitely
true, as there only has to exist 1 value for $x$ for this statement to be true,
and in part a we showed just that.

(c) This is false. The statement $\forall x P(x)$ is saying "For every possible
value in $x$, it is true that $17x + 1$ is even". That cannot be true. Just take
$P(2) = 35$ as a simple example. Basically when you start off with a $\forall$
predicate, every single value passed for $x$ (in this case) has to hold for the
assertion.

8.

Q: Let $P(x)$ be the predicate, "$18x + 1$ is even."

(a) Is $P(15)$ true or false?

(b) What, if anything, can you conclude about $\exists x P(x)$ from the truth
value of $P(15)$?

(c) What, if anything, can you conclude about $\forall x P(x)$ from the truth
value of $P(15)$?

A:

(a) Let's evaluate $P(15)$:

$$ P(15) = 18(15) + 1 = 271 $$

But obviously 271 is odd. This is a false statement.

(b) Because $18$ is an even number, and adding $1$ onto an even number will
always result in an odd number. We can conclude that the statement
$\exists x P(x)$, which means "There exists at least one value for $x$ where
$18x + 1$ is even." is false. There is no value for $x$ where $P(x)$ is true.

(c) The statement $\forall x P(x)$, which states "For every value of $x$,
$18x + 1$ is even" is also false. In fact, the exact opposite is true. As we
explained in part b, $P(x)$ can never be true for _any_ value of $x$. Thusly, to
state that it must be true for every possible value of $x$ as $\forall x P(x)$
asserts, simply cannot be the case.

9.

Q: Consider the sentence, $\exists x P(x, y) \to \forall x P(x, y)$. What can we
say about this sentence? Select all that apply.

A. The sentence is a statement because it contains quantifiers.

B. The sentence is not a statement because $x$ and $z$ are free variables.

C. The sentence is not a statement because $y$ is a free variable.

D. The universal generalization of the sentence is a statement.

A:

A. This is false, a sentence becomes a statement when a quantifier makes the
resulting statement true or false. But free variables still matter. The above
sentence essentially says "If there exists some value for $x$ where $P(x, y)$ is
true, then for every value for $x$, $P(x, y)$ must be true." But a sentence
cannot be a statement until, in this case, both $x$, and $y$ are replaced by
constants.

B. $z$ is never mentioned, so this statement is not true.

C. This is true. A statement cannot contain a free variable. Only when you
replace a free variable with a constant of some sort does a sentence become a
statement proper.

D. No, this statement is false. Although $x$ is bound by the universal
quantifier $\forall$, $y$ is not bound, and so remains a free variable. The
universal generalization of a sentence can only be a statement if the universal
quantifiers at the beginning of the sentence bind (restrict the domain) of all
free variables. $x$ is bound in this way after the predicate, but $y$ is not.

10.

Q: Suppose $P(x, y)$ is some binary predicate defined on a very small domain of
discourse: just the integers 1, 2, 3, 4. For each of the 16 pairs of these
numbers, $P(x, y)$ is either true or false, according to the following table
($x$ values are rows, $y$ values are columns).

|   | 1 | 2 | 3 | 4 |
| - | - | - | - | - |
| 1 | T | F | F | F |
| 2 | F | T | T | F |
| 3 | T | T | T | T |
| 4 | F | F | F | F |

For example, $P(1, 3)$ is false, as indicated by the $F$ in the first row, third
column. Use the table to decide whether the following statements are true or
false.

(a) $\forall y \exists x P(x, y)$.

(b) $\exists x \forall y P(x, y)$.

(c) $\forall x \exists y P(x, y)$.

(d) $\exists y \forall x P(x, y)$.

A:

(a) This is true. "For all columns, y, there exists some row, $x$, where
$P(x, y)$ returns true." This means that there must be some T somewhere in the
column.

$$ y = 1: T exists (1, 3) $$

$$ y = 4: T exists (4, 1) $$

(b) "There exists at least one row, $x$, where all of the column values, $y$,
return T."

This is true.

$$ x = 3: T exists (3, 1), (3, 2), (3, 3), (3, 4) $$

(c) "For all rows, $x$, there exists at least one column $y$, that returns T."

This is false, this is essentially saying every row has at least one T value,
but row 4 does not. Consider the following statement:

$$ x = 4: T \text{ exists in at least one of: } (4, 1), (4, 2), (4, 3), (4, 4) $$

This isn't true, row 4 returns all F.

(d) "There exists at least one column, $y$, where all rows $x$ return T"

This is false. There is no column $y$ where all rows are filled with Ts.
