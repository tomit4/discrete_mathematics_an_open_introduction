# Preview Activity

1.

Q: Consider the statement, "If Tommy doesn't eat his broccoli, then he will not
get any ice cream." Which of the following statements mean the same thing
(_i.e._, will be true in the same situations)? Select all that apply.

A. If Tommy does eat his broccoli, then he will get ice cream.

B. If Tommy gets ice cream, then he ate his broccoli.

C. If Tommy doesn't get ice cream, then he didn't eat his broccoli.

D. Tommy ate his broccoli and still didn't get any ice cream.

A:

Let's first establish:

$$ P = \text{Tommy doesn't eat his broccoli} $$

$$ Q = \text{He will not get any ice cream} $$

And also let's establish our truth tables as:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

A. If Tommy does eat his broccoli, then he will get ice cream.

This equates to the last row of the truth table above:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | F   | T         |

Or:

$$ \neg P \wedge \neg Q \to (P \to Q) $$

B. If Tommy gets ice cream, then he ate his broccoli.

The two rows where $Q$ is false are:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | F   | F         |
| F   | F   | T         |

As we can see, we don't know if Tommy ate his broccoli just because he got ice
cream.

C. If Tommy doesn't get ice cream, then he didn't eat his broccoli.

This is the case where $Q$ is true:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| F   | T   | T         |

And again, we do not know if Tommy ate his broccoli just because he didn't get
his ice cream (equivalent to part B).

D. Tommy ate his broccoli and still didn't get any ice cream.

These are all situations where $P$ is false:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | T   | T         |
| F   | F   | T         |

And Tommy didn't get any ice cream, so:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | T   | T         |

2.

Q: Suppose that your shady uncle offers you the following deal: If you loan him
your car, then he will bring you tacos. In which of the following situations
would it be fair to say that your uncle is a liar (_i.e._, that his statement
was false)? Select all that apply.

A. You loan him your car. He brings you tacos.

B. You loan him your car. He never buys you tacos.

C. You don't loan him your car. He still brings you tacos.

D. You don't loan him your car. He never brings you tacos.

A:

Let's first establish:

$$ P = \text{You loan your uncle your car} $$

$$ Q = \text{your uncle brings you tacos} $$

The assumption is:

$$ P \to Q $$

And our truth tables again are:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

A. You loan him your car. He brings you tacos.

So here, it would not be fair to say our uncle is a liar, because he fulfilled
the first row of the truth table:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |

Which makes sense. In essence, he made a promise and then delivered.

B. You loan him your car. He never buys you tacos.

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | F   | F         |

Here it makes sense to call our uncle a liar. We loaned him our car $P$, but he
never gave us tacos $Q$, so the assertion $P \to Q$ is false, and hence our
uncle is a liar.

C. You don't loan him your car. He still brings you tacos.

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | T   | T         |

While in the regular world, we would still call our uncle a liar, in the context
of discrete mathematics logic, we actually would say our uncle told us the truth
here.

While we never loaned our uncle our car, $P$, he still gave us tacos $Q$, and
the truth table tells us that $P \to Q$ is still true.

D. You don't loan him your car. He never brings you tacos.

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | F   | T         |

Well here it actually would make sense in the real world and in the mathematical
context to say our uncle is not a liar. We never fulfilled our promise to loan
him the car $P$, and he never gave us tacos $Q$, so $P \to Q$ makes sense both
from a daily life logical standpoint and also from a discrete math one.

3.

Q: Consider the _sentence_, "If $x \geq 10$, then $x^2 \geq 25$." This sentence
becomes a statement when we replace $x$ by a value, or "capture" the $x$ in the
scope of a quantifier. Which of the following claims are true (select all that
apply)?

A. If we replace $x$ by $15$, then the resulting statement is true. (Note,
$15^2 = 225$.)

B. If we replace $x$ by $3$, then the resulting statement is true.

C. If we replace $x$ by $6$, then the resulting statement is true.

D. The universal generalization ("for all $x$, if $x \geq 10$, then
$x^2 \geq 25$") is true.

E. There is a number we could replace $x$ with that makes the statement false.

A:

Again, let's say that:

$$ P(x) = x \geq 10 $$

$$ Q(x) = x^2 \geq 25 $$

And truth tables:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

A. If we replace $x$ by $15$, then the resulting statement is true. (Note,
$15^2 = 225$.)

Let's evaluate:

$$ P(x) = x \geq 10 $$

$$ Q(x) = x^2 \geq 25 $$

$$ P(15) = 15 \geq 10 \Rightarrow \text{True} $$

$$ Q(15) = 225 \geq 25 \Rightarrow \text{True} $$

| $P(15)$ | $Q(15)$ | $P(15) \to Q(15)$ |
| ------- | ------- | ----------------- |
| T       | T       | T                 |

This statement is true.

B. If we replace $x$ by $3$, then the resulting statement is true.

Let's evaluate:

$$ P(x) = x \geq 10 $$

$$ Q(x) = x^2 \geq 25 $$

$$ P(3) = 3 \geq 10 \Rightarrow \text{False} $$

$$ Q(3) = 9 \geq 25 \Rightarrow \text{False} $$

| $P(3)$ | $Q(3)$ | $P(3) \to Q(3)$ |
| ------ | ------ | --------------- |
| F      | F      | T               |

This statement is true.

C. If we replace $x$ by $6$, then the resulting statement is true.

Let's evaluate:

$$ P(x) = x \geq 10 $$

$$ Q(x) = x^2 \geq 25 $$

$$ P(6) = 6 \geq 10 \Rightarrow \text{False} $$

$$ Q(6) = 36 \geq 25 \Rightarrow \text{True} $$

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| F   | T   | T         |

This statement is true.

D. The universal generalization ("for all $x$, if $x \geq 10$, then
$x^2 \geq 25$") is true.

Since this is a universal generalization, this has nothing to do with $P(x)$ or
$Q(x)$, unless we explicitly define it as such. Without those definitions, this
is saying:

$$ \forall x \left(x \geq 10 \to \left(x^2 \geq 25\right)\right) $$

Given our previous definitions for $P(x)$ and $Q(x)$, we could rewrite this as:

$$ \forall x (P(x) \to Q(x)) $$

This is a true statement. Since $10^2 = 100$, and any larger values for $x$ is
guaranteed to be larger than $25$.

E. There is a number we could replace $x$ with that makes the statement false.

The intuition from part D indicates that this would have to be false, but let's
consider our truth table to be sure:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | F   | F         |

The only way an "if/then" statement in this context can be false is if the
hypothesis, $P$, is true, but the conclusion, $Q$, is false.

So this would actually be saying:

$$ \exists x \neg (P(x) \to Q(x)) $$

But this is not true, as long as the hypothesis holds true, then $Q(x)$ will
also hold true.

This statement is false.

4.

Q: Consider the statement, "If I see a movie, then I eat popcorn" (which happens
to be true). Based solely on your intuition of English, which of the following
statements mean the same thing? Select all that apply.

A. If I eat popcorn, then I see a movie.

B. If I don't eat popcorn, then I don't see a movie.

C. It is necessary that I eat popcorn when I see a movie.

D. To see a movie, it is sufficient for me to eat popcorn.

E. I only watch a movie if I eat popcorn.

A:

So in this question, we're asking to solely use our intuition of English...

A. If I eat popcorn, then I see a movie.

This isn't necessarily true, as the original statement only says that If I see a
movie that I then eat popcorn. This statement is saying that if I eat popcorn,
then I see a movie. The first statement does not imply the other (I could eat
popcorn and then do anything else).

B. If I don't eat popcorn, then I don't see a movie.

This is true, as the first statement says that if I see a movie, then I eat
popcorn. Therefore if I'm not eating popcorn, I could be doing anything at all,
but I am definitely not seeing a movie.

C. It is necessary that I eat popcorn when I see a movie.

While it is true that "If I see a movie, then I eat popcorn." Nothing about the
statement claims that it is _necessary_ that I eat popcorn when I see a movie,
only that it is true that when I see a movie, that I then eat popcorn.

In the context of discrete math though, this is equivalent to the original
statement.

D. To see a movie, it is sufficient for me to eat popcorn.

There is nothing in the original statement, "If I see a movie, then I eat
popcorn" that makes any claims about the _sufficiency_ for me to eat popcorn.

E. I only watch a movie if I eat popcorn.

This is equivalent to the original statement.

C & E are the answers.
