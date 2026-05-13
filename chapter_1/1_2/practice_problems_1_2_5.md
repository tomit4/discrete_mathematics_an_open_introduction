# 1.2.5 Practice Problems

1.

Q: In my safe is a sheet of paper with two shapes drawn on it in colored crayon.
One is a circle, and the other is a pentagon. Each shape is drawn in a single
color. Suppose you believe me when I tell you that, "If the circle is purple,
then the pentagon is orange." What do you therefore know about the truth value
of the following statements?

(a) The circle and the pentagon are both purple.

(b) The circle and the pentagon are both orange.

\(c\) The circle is not purple, or the pentagon is orange.

(d) If the pentagon is orange, then the circle is purple.

(e) If the pentagon is not orange, then the circle is not purple.

A:

Let $P$ be "The circle is purple" and $Q$ be "The pentagon is orange."

$$ P \to Q $$

For reference let's also pull up our truth table:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

(a) The circle and the pentagon are both purple.

This follows the truth table of:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | F   | F         |

So we therefore know that (a) is a false statement.

(b) The circle and the pentagon are both orange.

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | T   | T         |
| F   | F   | T         |

Note that we include both of these because since $P$ is false, it does not
matter if $Q$ is true, we only know that $P \to Q$ is true.

While $P \to Q$ is definitely true, we cannot determine if $Q$ is true or false,
and therefore the validity of statement (b) is unknown.

\(c\) The circle is not purple, or the pentagon is orange.

This equates to:

$$ \neg P \vee Q $$

Let's "flip" our values for $P$ in our truth table to reflect this:

| $\neg P$ | $Q$ | $P \to Q$ |
| -------- | --- | --------- |
| F        | T   | T         |
| F        | F   | F         |
| T        | T   | T         |
| T        | F   | T         |

And now isolate our statement in (c):

| $\neg P$ | $Q$ | $P \to Q$ |
| -------- | --- | --------- |
| T        | T   | T         |
| T        | F   | T         |

This is a true statement $P \to Q$, as it tells us that the circle is not
purple, and the pentagon _could_ be orange or not orange.

(d) If the pentagon is orange, then the circle is purple.

This is the converse statement to the implication.

$$ Q \to P $$

This is not true, we cannot know this to be true based off the implication. In
other words, just because the pentagon is orange does not _necessarily_ mean
that the circle is purple.

The statement (d) is unknown.

(e) If the pentagon is not orange, then the circle is not purple.

This is the contrapositive:

$$ \neg Q \to \neg P $$

As we know, the contrapositive is always true if the implication is true. Since
we established in the original problem statement that our implication is true,
the contrapositive must also be true.

2.

Q: Suppose the statement, "_If the square is yellow, then the circle is purple_"
is true. Assume also that the converse is false. Classify each statement below
as true or false (if possible).

(a) The circle is purple.

(b) The square is yellow if and only if the circle is not purple.

\(c\) The square is yellow.

(d) The square is yellow if and only if the circle is purple.

A:

So let's start with our implication:

Let $P$ be "The square is yellow", and the conclusion $Q$ be "The circle is
purple."

$$ P \to Q $$

We also know that the converse is false:

$$ \neg(Q \to P) $$

And again, our truth tables:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

(a) The circle is purple.

Since this is the predicate of the converse statement, then the only thing we
know to be true given our two assumptions is that the square is not yellow.
Ultimately though, we do not know if this is a true statement or not, so it is
not possible to classify this statement as either true or false.

(b) The square is yellow if and only if the circle is not purple.

This statement is saying:

$$ P \leftrightarrow \neg Q $$

But in order for this to be true, then both of the following statements would
also have to be true:

$$ P \to \neg Q $$

"If the square is yellow, then the circle is not purple."

$$ \neg Q \to P $$

"If the circle is not purple, then the square is yellow."

The first statement directly contradicts the implication and the second
statement is not known.

This statement is false due to the contradiction of the first statement with the
implication.

\(c\) The square is yellow.

We cannot know if this statement is true or not. If it is, then we know that the
circle is purple, but again, this statement cannot be classified as either true
or false.

(d) The square is yellow if and only if the circle is purple.

This statement is saying:

$$ P \leftrightarrow Q $$

This is false, in order for this statement to be true, both the implication as
well as its converse must be true, but the original problem statement tells us
the implication is true and the converse is false.

This statement is false.

3.

Q: Consider the statement, "_If you will give me magic beans, then I will give
you a cow._" Decide whether each statement below is the converse, the
contrapositive, or neither.

(a) If I will give you a cow, then you will not give me magic beans.

(b) If I will give you a cow, then you will give me magic beans.

\(c\) If you will not give me magic beans, then I will not give you a cow.

(d) If you will give me magic beans, then I will not give you a cow.

(e) You will give me magic beans, then I will not give you a cow.

(f) If I will not give you a cow, then you will not give me magic beans.

A:

Let $P$ be "You will give me magic beans" and $Q$ be "I will give you a cow."

And let us review definition 1.2.6:

Given an implication $P \to Q$, we say,

- The **converse** is the statement $Q \to P$.

- The **contrapositive** is the statement $\neg Q \to \neg P$.

- The **inverse** is the statement, $\neg P \to \neg Q$.

(a) If I will give you a cow, then you will not give me magic beans.

This equates to:

$$ Q \to \neg P $$

This does not correspond to any of our definitions.

(b) If I will give you a cow, then you will give me magic beans.

This equates to:

$$ Q \to P $$

This is the **converse** statement.

\(c\) If you will not give me magic beans, then I will not give you a cow.

This equates to:

$$ \neg P \to \neg Q $$

This is the **inverse** statement.

(d) If you will give me magic beans, then I will not give you a cow.

This equates to:

$$ P \to \neg Q $$

This does not correspond to any of the definitions.

(e) You will give me magic beans, then I will not give you a cow.

This equates to:

$$ P \to \neg Q $$

Which again, does not correspond to any of the definitions.

(f) If I will not give you a cow, then you will not give me magic beans.

This equates to:

$$ \neg Q \to \neg P $$

This is the **contrapositive** statement.

4.

Q: You have discovered an old paper on graph theory that discusses the
_viscosity_ of a graph (which for all you know, is something completely made up
by the author). A theorem in the paper claims that "if a graph satisfies
_condition_ _(V)_, then the graph is _viscous_." Which of the following are
equivalent ways of stating this claim? Which are equivalent to the converse of
the claim?

(a) Only viscous graphs satisfy condition (V).

(b) For a graph to be viscous, it is necessary that it satisfies condition (V).

\(c\) A graph is viscous only if it satisfies condition (V).

(d) Satisfying condition (V) is a necessary condition for a graph to be viscous.

(e) A graph is viscous if it satisfies condition (V).

A:

Let $P$ be "A graph satisfies condition (V)" and $Q$ be "the graph is viscous."

Let's also review the _converse_ definition:

Given an implication $P \to Q$, we say,

- The **converse** is the statement $Q \to P$.

And also let's also review necessary/sufficient wording definitions:

- "$P$ is necessary for $Q$" means $Q \to P$.

- "$P$ is sufficient for $Q$" means $P \to Q$.

- If $P$ is necessary and sufficient for $Q$, then $P \leftrightarrow Q$.

(a) Only viscous graphs satisfy condition (V).

This is:

$$ Q \to P $$

Which is equivalent to the _converse_ of the claim.

(b) For a graph to be viscous, it is necessary that it satisfies condition (V).

Recall the wording:

- "$P$ is necessary for $Q$" means $Q \to P$.

This is the _converse_ of the claim.

\(c\) A graph is viscous only if it satisfies condition (V).

- "$P$ is sufficient for $Q$" means $P \to Q$.

"only if it satisfies" usually says something along the lines of "I am $Q$ only
if I am $P$."

But again, statement \(c\) is saying $Q$ only if $P$, so it is reversed, so this
lines up as a **converse**.

This is equivalent to the _converse_ of the claim.

(d) Satisfying condition (V) is a necessary condition for a graph to be viscous.

- "$P$ is necessary for $Q$" means $Q \to P$.

And this is a direct wording to our (d) statement, so:

This is equivalent to the _converse_ of the claim.

(e) A graph is viscous if it satisfies condition (V).

This is the same as the original implication, just reversed, looking for the
"if" statement tells us which is $P$ and which is $Q$.

$$ P \to Q $$

This is an equivalent way of stating the original claim.

5.

Q: Which of the following statements are equivalent to the implication, "_if you
win the lottery, then you will be rich,_" and which are equivalent to the
converse of the implication?

(a) If you are not rich, then you did not win the lottery.

(b) It is sufficient to win the lottery to be rich.

\(c\) Either you win the lottery, or else you are not rich.

(d) If you are rich, you must have won the lottery.

(e) You will win the lottery if and only if you are rich.

A:

Let $P$ be "You win the lottery" and $Q$ be "You will be rich".

Let's also review the _converse_ definition:

Given an implication $P \to Q$, we say,

- The **converse** is the statement $Q \to P$.

And also let's also review necessary/sufficient wording definitions:

- "$P$ is necessary for $Q$" means $Q \to P$.

- "$P$ is sufficient for $Q$" means $P \to Q$.

- If $P$ is necessary and sufficient for $Q$, then $P \leftrightarrow Q$.

(a) If you are not rich, then you did not win the lottery.

This is:

$$ \neg Q \to \neg P $$

This is the _contrapositive_ of the implication statement, not the _converse_,
but it is always true if the implication is true. Therefore they are equivalent
statements.

(b) It is sufficient to win the lottery to be rich.

This is equivalent to the implication as:

- "$P$ is sufficient for $Q$" means $P \to Q$.

\(c\) Either you win the lottery, or else you are not rich.

This is saying:

$$ P \vee \neg Q $$

This is equivalent to:

$$ P \vee \neg Q \equiv Q \to P $$

This is the _converse_ statement.

(d) If you are rich, you must have won the lottery.

This is:

$$ Q \to P $$

This is the _converse_ of the implication.

(e) You will win the lottery if and only if you are rich.

This is:

$$ Q \leftrightarrow P $$

This is a bidirectional statement, which will only be true if both the
implication and its converse statement are true. It is not equivalent to either
the implication nor its converse.
