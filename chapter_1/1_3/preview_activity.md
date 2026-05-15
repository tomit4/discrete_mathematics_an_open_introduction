# Preview Activity

1.

Q: Consider the statement, "Whenever Holmes wears a purple shirt and the green
vest, he chooses to not wear a bow tie." Let $P$ be the statement, "Holmes wears
a purple shirt," $G$ be the statement, "Holmes wears the green vest," and $B$ be
the statement, "Holmes wears a bow tie." Which of the following is the best
translation of the statement into propositional logic?

A. $(P \wedge G) \to \neg B$

B. $P \wedge G \to B$

C. $(P \vee G) \to \neg B$

D. $P \vee (G \to B)$

A:

A. $(P \wedge G) \to \neg B$

This is the answer. $\wedge$ stands in for "and", and the given statement
declares that whenever Holmes wears a purple shirt, $P$ and the green vest, $G$
($P \wedge G$), then he chooses to not wear a bow tie $\to \neg B$.

B. $P \wedge G \to B$

This does not translate properly, what this implies is that "Whenever Holmes
wears a purple shirt and the green vest, he chooses to wear a bow tie." But the
problem statement explicitly declares that Holmes does _not_ wear a bow tie if
he is wearing a purple shirt and the green vest.

C. $(P \vee G) \to \neg B$

This also does not translate properly, this would be "Whenever Holmes wears a
purple shirt or the green vest, he chooses to not wear a bow tie."

D. $P \vee (G \to B)$

This one's a bit more difficult to translate, but also is not the best
translation. This essentially says "Either Holmes wears a purple shirt, or if
Holmes wears a green vest, he wears a bow tie."

2.

Q: Consider the statement, "Holmes never wears the green vest unless he is also
wearing either a purple shirt or red shoes." With $P$ and $G$ as in the previous
question, and $R$ being the statement, "Holmes wears red shoes," which of the
following is the best translation of the statement into propositional logic?

A. $G \to (P \vee R)$

B. $\neg G \to (P \vee R)$

C. $(P \vee R) \to G$

D. $(P \vee R) \to \neg G$

A:

A. $G \to (P \vee R)$

This is equivalent to the given statement. This is saying "If Holmes is wearing
the green vest, then he is either wearing a purple shirt or red shoes."

B. $\neg G \to (P \vee R)$

This is not the best translation, although the $\neg G$ makes it appear so. What
this is saying is "Whenever Holmes is not wearing the green vest, then he is
either wearing a purple shirt or red shoes."

C. $(P \vee R) \to G$

This appears to be the same as part A, but if we state this out carefully, this
says "If Holmes wears either the purple shirt or the red shoes, then he is
wearing the green vest." That is not the same as the given statement.

D. $(P \vee R) \to \neg G$

This is the same as part C, but it implies the opposite. "If Holmes is wearing
either the purple shirt or the red shoes, then he is not wearing the green
vest." Which is also not the same as the given statement.

3.

Q: Consider the statement, "If you major in math, then you will get a
high-paying job," and the statement, "Either you don't major in math, or you
will get a high-paying job." In which of the following cases are _both_
statements true?

A. You major in math and get a high-paying job.

B. You major in math and don't get a high-paying job.

C. You don't major in math and do get a high-paying job.

D. You don't major in math and don't get a high-paying job.

A :

Let $P$ be "You major in math" and $Q$ be "You get a high-paying job."

The first given statement then is:

$$ P \to Q $$

The second statement is:

$$ \neg P \vee Q $$

These are logically equivalent if you think about it.

$P \to Q$ is false if $P$ is true and $Q$ is false.

$\neg P \vee Q$ is false if $P$ is true and $Q$ is false.

With this in mind, let's answer each section.

A. You major in math and get a high-paying job.

$P = \text{ T}$

$Q = \text{ T}$

$$ P \to Q = T \to T = T $$

$$ \neg P \vee Q = F \vee T = T $$

This is a case where both statements are true.

B. You major in math and don't get a high-paying job.

$P = \text{ T}$

$Q = \text{ F}$

$$ P \to Q = T \to F = F $$

$$ \neg P \vee Q = F \vee F = F $$

Both are false, so this is not a case where both statements are true.

C. You don't major in math and do get a high-paying job.

$P = \text{ F}$

$Q = \text{ T}$

$$ P \to Q = F \to T = T $$

$$ \neg P \vee Q = T \vee T = T $$

This is a case where both statements are true.

D. You don't major in math and don't get a high-paying job.

$P = \text{ F}$

$Q = \text{ F}$

$$ P \to Q = F \to F = T $$

$$ \neg P \vee Q = T \vee F = T $$

Both statements are true, this is a case.

The answer is A, C, and D.
