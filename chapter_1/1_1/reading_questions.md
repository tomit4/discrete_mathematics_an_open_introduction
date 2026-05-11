1.

Q: Match each statement in symbols with it stype of statement.

|              |                                 |
| ------------ | ------------------------------- |
| $P \to Q$    | $P$ and $Q$ (conjunction)       |
| $P \vee Q$   | If $P$, then $Q$, (implication) |
| $P \wedge Q$ | $P$ or $Q$ (disjunction)        |
| $\neg P$     | Not $P$ (negation)              |

A:

|              |                                 |
| ------------ | ------------------------------- |
| $P \to Q$    | If $P$, then $Q$, (implication) |
| $P \wedge Q$ | $P$ and $Q$ (conjunction)       |
| $P \vee  Q$  | $P$ or $Q$ (disjunction)        |
| $\neg P$     | Not $P$ (negation)              |

2.

Q: Consider the sentence, "If $x > 3$, then $x$ is even."

Which of the following statements are true about the sentence? Select all that
apply.

    A. The sentence is a false statement since it has a free variable.

    B. The universal generalization of the sentence is a statement.

    C. If you substitute 10 for $x$, the resulting statement is true.

    D. The sentence becomes a true statement no matter what natural number you substitute for $x$.

A:

B and C are true about the sentence.

A. No, this sentence is not a statement because it has a free variable, but that
doesn't automatically make the statement true or false.

B. Given a sentence with free variables, the **universal generalization** of a
sentence is the statement obtained by adding enough universal quantifiers to the
beginning of the sentence so that all free variables become bound.

The beginning of the sentence states "If $x > 3$", this is a universal
quantifier that bounds our free variable, $x$, and therefore by the definition
of the **universal generalization**, this sentence is therefore a statement.

C. This is also true, though it doesn't follow in "regular" day to day logic,
but recall our truth table for $P \to Q$:

| $P$ | $Q$ | $P \to $Q$ |
| --- | --- | ---------- |
| T   | T   | T          |

Again our sentence is:

"If $x > 3$, then $x$ is even."

We can say that $P(x)$ is "If $x > 3$", and that $Q(x)$ is "$x$ is even."

$$ P(x) \to Q(x) $$

Since $x = 10$ according to C, this means that:

$$ P(10) = \text{ If }10 > 3 = \text{ True} $$

$$ Q(10) = 10 \text{ is even} = \text{ True} $$

So therefore it follows that:

$$ P(10) \to Q(10) $$

Is a true statement.

3. What questions do you have after reading this section? Write at least one
   question about the content of this section that you are curious about.

This section is quite interesting, I suppose I'm curious about how negation
adjusts the truth tables of other qualifiers. In one of the examples, this
statement is made:

17 is not prime if and only if 19 is not prime.

To which the answer is:

True. Now both parts are false (since both are the negation of a true
statement), so the entire statement is true.

The $P \leftrightarrow Q$ statement does confuse me, and so therefore we have:

$$ \neg P \leftrightarrow \neg Q $$

and I suppose I just need to sit down and have some clarification on how
negation affects this statement.
