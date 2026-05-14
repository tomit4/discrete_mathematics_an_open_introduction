# 1.3.3 Logical Equivalence

You might have noticed in Example 1.3.2 that the final column in the truth table
for $\neg P \vee Q$ is identical to the final column in the truth table for
$P \to Q$:

| $P$ | $Q$ | $P \to Q$ | $\neg P \vee Q$ |
| --- | --- | --------- | --------------- |
| T   | T   | T         | T               |
| T   | F   | F         | F               |
| F   | T   | T         | T               |
| F   | F   | T         | T               |

This says that no matter what $P$ and $Q$ are, the statements $\neg P \vee Q$
and $P \to Q$ are either both true or both false. We therefore say these
statements are **logically equivalent**.

---

## Definition 1.3.4 Logical Equivalence

Two (molecular) statements $P$ and $Q$ are **logically equivalent** provided $P$
is true precisely when $Q$ is true. That is, $P$ and $Q$ have the same truth
value under any assignment of truth values to their atomic parts. We write this
as $P \equiv Q$.

---

To verify that two statements are logically equivalent, you can make a truth
table for each and check whether the columns for the two statements are
identical.

In Section 1.2 we claimed that whenever an implication is true, so is its
contrapositive. We can now make this claim as the following theorem.

## Theorem 1.3.5

_An implication is logically equivalent to its contrapositive. That is,_

$$ P \to Q \equiv \neg Q \to \neg P $$

**Proof**

We simply examine the truth tables.

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

| $P$ | $Q$ | $\neg Q$ | $\neg P$ | $\neg Q \to \neg P$ |
| --- | --- | -------- | -------- | ------------------- |
| T   | T   | F        | F        | T                   |
| T   | F   | T        | F        | F                   |
| F   | T   | F        | T        | T                   |
| F   | F   | T        | T        | T                   |

(Note that we have the truth value combinations in the same order in both
tables, so we can easily see that the final columns are identical)

(Note that we have the truth value combinations in the same order in both
tables, so we can easily see that the final columns are identical)

Recognizing two statements as logically equivalent can be quite helpful.
Rephrasing a mathematical statement can often lend insight into what it is
saying, or how to prove or refute it. By using truth tables we can
systematically verify that two statements are indeed logically equivalent.
