# 1.3.7 Practice Problems

1.

Q: Make a truth table for the statement $(P \wedge Q) \to (P \vee Q)$.

A:

| $P$ | $Q$ | $(P \wedge Q)$ | $(P \vee Q)$ | $(P \wedge Q) \to (P \vee Q)$ |
| --- | --- | -------------- | ------------ | ----------------------------- |
| T   | T   | T              | T            | T                             |
| T   | F   | F              | T            | T                             |
| F   | T   | F              | T            | T                             |
| F   | F   | F              | F            | T                             |

2.

Q: Complete a truth table for the statement $\neg Q \vee (Q \to P)$. What can
you conclude about $P$ and $Q$ if you knew the statement above was false?

| $Q$ | $P$ | $\neg Q$ | $Q \to P$ | $\neg Q \vee (Q \to P)$ |
| --- | --- | -------- | --------- | ----------------------- |
| T   | T   | F        | T         | T                       |
| T   | F   | F        | F         | F                       |
| F   | T   | T        | T         | T                       |
| F   | F   | T        | T         | T                       |

If we know that $\neg Q \to \vee (Q \to P)$ is false, then the only possible
values are $Q = T$ and $P = F$.

3. Construct a truth table for the statement $Q \to (\neg P \vee R)$.

| $P$ | $Q$ | $R$ | $\neg P$ | $(\neg P \vee R)$ | $Q \to (\neg P \vee R)$ |
| --- | --- | --- | -------- | ----------------- | ----------------------- |
| T   | T   | T   | F        | T                 | T                       |
| T   | T   | F   | F        | F                 | F                       |
| T   | F   | T   | F        | T                 | T                       |
| T   | F   | F   | F        | F                 | T                       |
| F   | T   | T   | T        | T                 | T                       |
| F   | F   | T   | T        | T                 | T                       |
| F   | T   | F   | T        | T                 | T                       |
| F   | F   | F   | T        | T                 | T                       |

4.

Q: Determine whether the statements $P \to (Q \vee R)$ and
$(P \to Q) \vee (P \to R)$ are logically equivalent by completing a truth table
for both statements.

A:

| $P$ | $Q$ | $R$ | $(Q \vee R)$ | $(P \to Q)$ | $(P \to R)$ | $P \to (Q \vee R)$ | $(P \to Q) \vee (P \to R)$ |
| --- | --- | --- | ------------ | ----------- | ----------- | ------------------ | -------------------------- |
| T   | T   | T   | T            | T           | T           | T                  | T                          |
| T   | T   | F   | T            | T           | F           | T                  | F                          |
| T   | F   | T   | T            | F           | T           | T                  | T                          |
| T   | F   | F   | F            | F           | F           | F                  | F                          |
| F   | T   | T   | T            | T           | T           | T                  | T                          |
| F   | T   | F   | T            | T           | T           | T                  | T                          |
| F   | F   | T   | T            | T           | T           | T                  | T                          |
| F   | F   | F   | F            | T           | T           | T                  | T                          |

From this truth table, we can conclude that the statements $P \to (Q \vee R)$
and $(P \to Q) \vee (P \to R)$ are _not_ logically equivalent statements.

5.

Determine if the following is a valid deduction rule:

$$
P \to Q \\
\neg Q \\
\overline{\therefore \quad \neg P}
$$

We can first construct a truth table:

| $P$ | $Q$ | $\neg Q$ | $P \to Q$ | $\neg P$ |
| --- | --- | -------- | --------- | -------- |
| T   | T   | F        | T         | F        |
| T   | F   | T        | F         | F        |
| F   | T   | F        | T         | T        |
| F   | F   | T        | T         | T        |

The last row shows us that this is a valid deduction, where the conclusion,
$\neg Q$ is true and the two premises, $P \to Q$ and $\neg P$ are both true as
well. While this is the only row where the premises are both true, if there were
other rows where the premises were both true, we would then check to see if the
conclusion was true as well. Only if all the rows all had the premises as being
true as well as the conclusion being true could we say that this is a valid
deduction.

Since we only have one row where both premises are true though, we only check
this one, which is valid. This is a valid deduction.

6. Determine if the following is a valid deduction rule:

$$
P \to (Q \vee R) \\
\neg (P \to Q) \\
\overline{\therefore \quad R}
$$

| $P$ | $Q$ | $R$ | $(Q \vee R)$ | $(P \to Q)$ | $P \to (Q \vee R)$ | \neg(P \to Q) |
| --- | --- | --- | ------------ | ----------- | ------------------ | ------------- |
| T   | T   | T   | T            | T           | T                  | F             |
| T   | T   | F   | T            | T           | T                  | F             |
| T   | F   | T   | T            | F           | T                  | T             |
| T   | F   | F   | F            | F           | F                  | T             |
| F   | T   | T   | T            | T           | T                  | F             |
| F   | T   | F   | T            | T           | T                  | F             |
| F   | F   | T   | T            | T           | T                  | F             |
| F   | F   | F   | F            | T           | T                  | F             |

Let's now isolate the rows where the premises $P \to (Q \vee R)$ and
$\neg (P \to Q)$ are both true:

| $P$ | $Q$ | $R$ | $(Q \vee R)$ | $(P \to Q)$ | $P \to (Q \vee R)$ | \neg(P \to Q) |
| --- | --- | --- | ------------ | ----------- | ------------------ | ------------- |
| T   | F   | T   | T            | F           | **T**              | **T**         |

Now let's see if within these remaining rows if $R$ is true:

| $P$ | $Q$ | $R$   | $(Q \vee R)$ | $(P \to Q)$ | $P \to (Q \vee R)$ | \neg(P \to Q) |
| --- | --- | ----- | ------------ | ----------- | ------------------ | ------------- |
| T   | F   | **T** | T            | F           | **T**              | **T**         |

Since the only row where both premises $P \to (Q \vee R)$ and $\neg(P \to Q)$
are true also has $R$ true, this is a valid deduction rule.

7. Determine if the following is a valid deduction rule:

$$
(P \wedge Q) \to R \\
\neg P \vee \neg Q \\
\overline{\therefore \neg R}
$$

| $P$ | $Q$ | $R$ | $(P \wedge Q)$ | $(P \wedge Q) \to R$ | $\neg P$ | $\neg Q$ | $\neg P \vee \neg Q$ | $\neg R$ |
| --- | --- | --- | -------------- | -------------------- | -------- | -------- | -------------------- | -------- |
| T   | T   | T   | T              | T                    | F        | F        | F                    | F        |
| T   | T   | F   | T              | F                    | F        | F        | F                    | T        |
| T   | F   | T   | F              | T                    | F        | T        | T                    | F        |
| T   | F   | F   | F              | T                    | F        | T        | T                    | T        |
| F   | T   | T   | F              | T                    | T        | F        | T                    | F        |
| F   | T   | F   | F              | T                    | T        | F        | T                    | T        |
| F   | F   | T   | F              | T                    | T        | T        | T                    | F        |
| F   | F   | F   | F              | T                    | T        | T        | T                    | T        |

Let's now isolate the rows where the premises $(P \wedge Q) \to R$ and
$\neg P \vee \neg Q$ are both true:

| $P$ | $Q$ | $R$ | $(P \wedge Q)$ | $(P \wedge Q) \to R$ | $\neg P$ | $\neg Q$ | $\neg P \vee \neg Q$ | $\neg R$ |
| --- | --- | --- | -------------- | -------------------- | -------- | -------- | -------------------- | -------- |
| T   | F   | T   | F              | T                    | F        | T        | T                    | F        |
| T   | F   | F   | F              | T                    | F        | T        | T                    | T        |
| F   | T   | T   | F              | T                    | T        | F        | T                    | F        |
| F   | T   | F   | F              | T                    | T        | F        | T                    | T        |
| F   | F   | T   | F              | T                    | T        | T        | T                    | F        |
| F   | F   | F   | F              | T                    | T        | T        | T                    | T        |

Now let's see if within these remaining rows if all values for $\neg R$ are
true...they are not, so this is not a valid deduction rule.

8. Determine if the following is a valid deduction rule:

$$
P \to Q \\
P \wedge \neg Q \\
\overline{\therefore R}
$$

| $P$ | $Q$ | $R$ | $\neg Q$ | $P \to Q$ | $P \wedge \neg Q$ |
| --- | --- | --- | -------- | --------- | ----------------- |
| T   | T   | T   | F        | T         | F                 |
| T   | T   | F   | F        | T         | F                 |
| T   | F   | T   | T        | F         | T                 |
| T   | F   | F   | T        | F         | T                 |
| F   | T   | T   | F        | T         | F                 |
| F   | T   | F   | F        | T         | F                 |
| F   | F   | T   | T        | T         | F                 |
| F   | F   | F   | T        | T         | F                 |

Now, let's isolate the rows where the premises $P \to Q$ and $P \wedge \neg Q$
are true:

| $P$ | $Q$ | $R$ | $\neg Q$ | $P \to Q$ | $P \wedge \neg Q$ |
| --- | --- | --- | -------- | --------- | ----------------- |
| T   | T   | T   | F        | T         | F                 |
| T   | T   | F   | F        | T         | F                 |
| F   | T   | T   | F        | T         | F                 |
| F   | T   | F   | F        | T         | F                 |
| F   | F   | T   | T        | T         | F                 |
| F   | F   | F   | T        | T         | F                 |

As you can see, in the remaining rows after isolating all rows where $P \to Q$
is true, all rows for $P \wedge \neg Q$ are false. In order to have a valid
deduction rule, all premises must first be true, and then the corresponding
conclusion must also be true. Since both premises are not valid in every
remaining case, there is no case to test the conclusion against. No
counterexamples exist. Since there are no cases where all premises are true but
the conclusion is false, this means that the given statement is
[vacuously valid](https://en.wikipedia.org/wiki/Vacuous_truth) and is therefore
a valid deduction rule.

9.

Q: Which of the following statements is a _law of logic_? That is, which of the
following are true no matter what your domain of discourse is and no matter what
you interpret the predicates as meaning? Select all that apply.

A: $\forall x (P(x) \vee \neg P(x))$.

B. $\exists x P(x) \to \forall x P(x)$.

C. $\neg \forall x P(x) \to \exists x P(x)$.

D. $\forall x \exists y P(x, y) \leftrightarrow \exists y \forall x P(x, y)$.

A:

A law of logic is a statement in predicate logic that is necessarily true.

A: $\forall x (P(x) \vee \neg P(x))$.

This statement does follow the law of logic. It is saying "For all things $x$,
some fact $P(x)$ is true or that same fact, $P(x)$ is not true." In extremely
basic English, "All things are either something or not something."

B. $\exists x P(x) \to \forall x P(x)$.

This statement does _not_ follow the law of logic. It is saying "If there exists
some thing, $x$, for which there is some truth $P(x)$, then for all things that
are $x$, that truth $P(x)$ is true." This is not necessarily true.

C. $\neg \forall x P(x) \to \exists x P(x)$.

This statement does _not_ follow the law of logic. It is saying "For all things
$x$, if $P(x)$ is not true, then there exists at least one $x$ for which $P(x)$
is true." A more accurate statement would be:

$$ \neg \forall x P(x) \to \exits x \neg P(x) $$

This one tripped me up, so for notations sake, let's say $P(x)$ means "person
$x$ cares". So the statement given in C would become "If nobody cares, then
there exists at least someone who cares." Which isn't true, there could truly be
0 people who care.

The last statement I gave that is more accurate would be saying "If nobody
cares, then there exists at least one person who doesn't care."

D. $\forall x \exists y P(x, y) \leftrightarrow \exists y \forall x P(x, y)$.

"For all things $x$, there is at least one $y$ where $P(x, y)$ is true if and
only if there exists at least one $y$ for every $x$ that $P(x, y)$ is true."

These do not follow the law of logic, but to understand it's best to define $x$
and $y$ in some context.

Let $x$ be "boss" and $y$ be "employee", and $P(x, y)$ be "boss is an employer
of an employee."

The first statement would be:

"For all bosses, there exists at least one employee for which the boss is an
employer of an employee."

The second statement would be:

"There exists at least one employee for all bosses for which the boss is an
employer of an employee."

The first statement is true, but the second statement is false, an "if and only
if" statement is true only if both statements are true or both statements are
false.
