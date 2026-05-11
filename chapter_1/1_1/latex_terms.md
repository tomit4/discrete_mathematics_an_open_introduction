## Definition 1.1.7 Logical Connectives.

We define the following **logical connectives.**

- $P \wedge Q$ is read "P and Q", and is called a **conjunction**.

- $P \vee Q$ is read "P or Q", and is called a **disjunction**.

- $P \to Q$ is read "if P then Q", and is called an **implication** or
  **conditional**.

- $P \leftrightarrow Q$ is read "P if and only if Q" and is called a
  **biconditional**.

- $$ \neg P $$
  is read "not P", and is called a **negation**.

## Definitions 1.1.8 Truth Conditions for Connectives.

The **truth conditions** for the logical connectives are defined as follows.

- $P \wedge Q$ is true when both $P$ and $Q$ are true.

- $P \vee Q$ is trueh when $P$ or $Q$ or both are true.

- $P \to Q$ is true when $P$ is false or $Q$ is true (or both).

- $P \leftrightarrow Q$ is true when $P$ and $Q$ are both true, or both false.

- $\neg P$ is true when $P$ is false.

**Personal Notes**

The statement $P \to Q$ was confusing for me. ChatGPT expalains it as:

The rule given in your book is:

$P \to Q$ is true when $P$ is false, or $Q$ is true (or both).

That sounds weird, so let’s rephrase:

The only time “If P, then Q” is false is if P happens but Q doesn’t happen. In
every other situation, the statement is considered true.

Think of it as a promise:

“If I do X, then Y will happen.”

The promise is broken only if I do X and Y fails to happen. Otherwise, the
promise hasn’t been broken.

Step 3:

Truth table example

| P (It rains) | Q (Ground wet) | P → Q (If it rains, then ground gets wet)       |
| ------------ | -------------- | ----------------------------------------------- |
| True         | True           | True (rain happened, ground got wet ✅)         |
| True         | False          | False (rain happened, ground stayed dry ❌)     |
| False        | True           | True (didn’t rain, but ground is wet anyway ✅) |
| False        | False          | True (didn’t rain, ground isn’t wet ✅)         |

Notice that whenever it didn’t rain ($P$ is false), we consider the statement
“If it rains, then the ground gets wet” as true, because the promise about rain
hasn’t been broken.

## Definition 1.1.12 Quantifiers

The **universal quantifier** is written as $\forall$ and is read, "for all." The
**existential quantifier** is written $\exists$ and is read, "there exists" or
"for some."
