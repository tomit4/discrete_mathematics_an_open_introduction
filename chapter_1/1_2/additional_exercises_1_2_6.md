# 1.2.6 Additional Exercises

1.

Q: Translate into English:

(a) $\forall x (E(x) \to E(x + 2))$.

(b) $\forall x \exists y (\sin(x) = y)$.

\(c\) $\forall y \exists x (\sin(x) = y)$.

(d) $\forall x \forall y \left(x^3 = y^3 \to x = y\right)$.

A:

(a) $\forall x (E(x) \to E(x + 2))$.

For all numbers $x$, If $x$ is an even number, then it is true that $x + 2$ is
an even number.

(b) $\forall x \exists y (\sin(x) = y)$.

For all numbers $x$, there exists at least one number $y$ where $\sin(x) = y$.

\(c\) $\forall y \exists x (\sin(x) = y)$.

For all numbers $y$, there exits at least one number $x$ where $\sin(x) = y$.

(d) $\forall x \forall y \left(x^3 = y^3 \to x = y\right)$.

For all numbers $x$ and for all numbers $y$, it is true that if $x^3 = y^3$,
then it is true that $x = y$.

2.

Q: Consider the statement, "If Oscar eats Chinese food, then he drinks milk."

(a) Write the converse statement.

(b) Write the contrapositive of the statement.

\(c\) Is it possible for the contrapositive to be false? If it was, what would
that tell you?

(d) Suppose the original statement is true, and that Oscar drinks milk. Can you
conclude anything (about his eating Chinese food)? Explain.

(e) Suppose the original statement is true, and that Oscar does not drink milk.
Can you conclude anything (about his eating Chinese food)? Explain.

A:

Let $P$ be "Oscar eats Chinese food" and $Q$ be "Oscar drinks milk."

$$ P \to Q $$

Let's also review our statements:

Given an implication $P \to Q$, we say,

- The **converse** is the statement $Q \to P$.

- The **contrapositive** is the statement $\neg Q \to \neg P$.

- The **inverse** is the statement, $\neg P \to \neg Q$.

(a) Write the converse statement.

The converse statement is:

$$ Q \to P $$

In plain English it reads as: "If Oscar drinks milk, then he eats Chinese food."

(b) Write the contrapositive of the statement.

The contrapositive statement is $\neg Q \to \neg P$.

In plain English it reads as: "If Oscar does not drink milk, then he does not
eat Chinese food."

\(c\) Is it possible for the contrapositive to be false? If it was, what would
that tell you?

Yes, it is possible for the contrapositive to be false, but then the original
implication must also be false.

(d) Suppose the original statement is true, and that Oscar drinks milk. Can you
conclude anything (about his eating Chinese food)? Explain.

Consider our truth tables:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

Specifically where we know $Q$ is true:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| F   | T   | T         |

We can see here that we cannot know whether Oscar ate Chinese food $P$, simply
because we know that he drank milk $Q$, even though the statement $P \to Q$ is
true in either case.

(e) Suppose the original statement is true, and that Oscar does not drink milk.
Can you conclude anything (about his eating Chinese food)? Explain.

Again, let us consult our truth tables where $Q$ is false:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | F   | F         |
| F   | F   | T         |

But we know that $P \to Q$ is true as it is stated in the problem statement, so:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | F   | T         |

And so we _can_ conclude that if $P \to Q$ is true, and $Q$ is false, then we
know that $P$ is false as well. In other words, we can conclude that Oscar did
not eat Chinese food.

3.

Q: Write each of the following statements in the form, "If ..., then...."
Careful, some statements may be false (which is fine for the purposes of this
question).

(a) To lose weight, you must exercise.

(b) To lose weight, all you need to do is exercise.

\(c\) Every American is patriotic.

(d) You are patriotic only if you are American.

(e) The set of rational numbers is a subset of the real numbers.

(f) A number is prime if it is not even.

(g) Either the Broncos will win the Super Bowl, or they won't play in the Super
Bowl.

A:

(a) To lose weight, you must exercise.

"If you are to lose weight, then it is necessary for you to exercise."

(b) To lose weight, all you need to do is exercise.

"If you exercise, then you will lose weight."

\(c\) Every American is patriotic.

"If you are an American, then you are patriotic."

(d) You are patriotic only if you are American.

"If you are patriotic, then you must be an American."

(e) The set of rational numbers is a subset of the real numbers.

"If a number is in the set of rational numbers, then it is in the set of real
numbers."

(f) A number is prime if it is not even.

"If a number is prime, then it is not even."

(g) Either the Broncos will win the Super Bowl, or they won't play in the Super
Bowl.

$$ P \vee \neg Q \equiv Q \to P $$

"If the Broncos play in the Super Bowl, then the Broncos win the Super Bowl."

4.

Q: Consider the implication, "If you clean your room, then you can watch TV."
Rephrase the implication in as many ways as possible. Then do the same for the
converse.

A:

"If you clean your room, then you can watch TV."

Rephrasing of original implication:

1. You can watch TV if you clean your room.

2. You clean your room only if you can watch TV.

3. In order to watch TV, you must clean your room.

4. To watch TV, it is necessary that you clean your room.

5. To watch TV, it is sufficient to clean your room.

6. You did not clean your room unless you can watch TV.

And the converse:

"If you can watch TV, then you clean your room."

1. You clean your room if you can watch TV.

2. It is necessary that you clean your room in order for you to watch TV.

3. If you don't clean your room, then you cannot watch TV.

---

5.

Q: Recall from calculus, if a function is differentiable at a point $c$, then it
is continuous at $c$, but that the converse of this statement is not true (for
example, $f(x) = |x|$ at the point 0). Restate this fact using "necessary and
sufficient language."

A:

Let us recall:

- "$P$ is necessary for $Q$" means $Q \to P$.

- "$P$ is sufficient for $Q$" means $P \to Q$.

- If $P$ is necessary and sufficient for $Q$, then $P \leftrightarrow Q$.

Let $P$ be "A function is differentiable at a point $c$" and $Q$ be "the
function is continuous at point $c$." Therefore we can say:

- "$P$ is necessary for $Q$" means $Q \to P$ (this is false in this case).

"Continuity is necessary but not sufficient for differentiability at $c$."

- "$P$ is sufficient for $Q$" means $P \to Q$.

"Differentiability is sufficient for continuity."

- If $P$ is necessary and sufficient for $Q$, then $P \leftrightarrow Q$.

"Continuity is necessary but not sufficient for differentiability at $c$."

6.

Q: Consider the statement, "For all natural numbers $n$, if $n$ is prime, then
$n$ is solitary." You do not need to know what _solitary_ means for this
problem, just that it is a property that some numbers have and others do not.

(a) Write the converse and the contrapositive of the statement, saying which is
which. Note: the original statement claims that an implication is true for all
$n$, and it is that implication that we are taking the converse and
contrapositive of.

(b) Write the negation of the original statement. What would you need to show to
prove that the statement is false?

\(c\) Even though you don't know whether 10 is solitary (in fact, nobody knows
this), is the statement, "If 10 is prime, then 10 is solitary" true or false?
Explain.

(d) It turns out that 8 is solitary. Does this tell you anything about the truth
or fasilty of the original statement, its converse or its contrapositive?
Explain.

(e) Assuming that the original statement is true, what can you say about the
relationship between the _set_ $P$ of prime numbers and the _set_ $S$ of
solitary numbers. Explain.

A:

Let's first express this:

$$ \forall n (P(n) \to S(n)) $$

Let's also review our quantified converse/contrapositive definitions:

A quantified implication $\forall x (P(x) to Q(x))$ has:

**Converse** $\forall x(Q(x) \to P(x))$

**Contrapositive** $\forall x \left(\neg Q(n) \to \neg P(x)\right)$

(a) Write the converse and the contrapositive of the statement, saying which is
which. Note: the original statement claims that an implication is true for all
$n$, and it is that implication that we are taking the converse and
contrapositive of.

**Converse** $\forall n(S(n) \to P(n))$

"For all natural numbers $n$, if $n$ is solitary, then $n$ is prime."

**Contrapositive** $\forall n \left(\neg S(n) \to \neg P(n)\right)$

"For all natural numbers $n$, if $n$ is not solitary, then $n$ is not prime."

(b) Write the negation of the original statement. What would you need to show to
prove that the statement is false?

$$ \neg \forall n (P(n) \to S(n)) $$

To prove that this statement is false, there would have to exist at least one
value for $n$ where $n$ is prime and $n$ is not solitary.

$$ \exists n \neg (P(n) \to S(n)) $$

\(c\) Even though you don't know whether 10 is solitary (in fact, nobody knows
this), is the statement, "If 10 is prime, then 10 is solitary" true or false?
Explain.

This falls within our truth table as:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |

We cannot know if 10 is solitary or not as stated in the problem statement. We
only know that 10 is prime. So therefore we do not know if the statement
$P \to Q$, or "If 10 is prime, then 10 is solitary", is true or not.

(d) It turns out that 8 is solitary. Does this tell you anything about the truth
or falsity of the original statement, its converse or its contrapositive?
Explain.

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| F   | T   | T         |

Yes, this tells us that since we know that 8 is solitary, it does not matter if
8 is prime or not. Either way, "If 8 is prime, then 8 is solitary" ($P \to Q$),
is a true statement.

- The **converse** is the statement $Q \to P$.

In this context this means "If 8 is solitary, then 8 is prime" ($Q \to P$), if
we then invert the truth table, we get (where we know $Q$ is true):

| $Q$ | $P$ | $Q \to P$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |

And we cannot verify the truth or falsity of $Q \to P$ nor the truth or falsity
of $P$.

- The **contrapositive** is the statement $\neg Q \to \neg P$.

This must be true if the original implication is true. This is a true statement.

(e) Assuming that the original statement is true, what can you say about the
relationship between the _set_ $P$ of prime numbers and the _set_ $S$ of
solitary numbers. Explain.

We are given the statement:

$$ \forall n (P(n) \to S(n)) $$

This says that for every natural number $n$, if $n$ is prime, then $n$ is
solitary. In other words, every prime number has the property of being solitary.

We can interpret this in terms of sets as saying that every element of the set
of prime numbers is also an element of the set of solitary numbers. Therefore,
the set of prime numbers is a subset of the set of solitary numbers:

$$ P \subseteq S $$
