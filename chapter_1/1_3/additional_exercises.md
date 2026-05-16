# 1.3.8 Additional Exercises

1.

Q: You stumble upon two trolls playing Stratego. They tell you:

Troll 1: If we are cousins, then we are both knaves.

Troll 2: We are cousins, or we are both knaves.

Could both trolls be knights? Recall that all trolls are either
always-truth-telling knights or always-lying knaves. Explain your answer and how
you can use truth tables to find it.

Let $P$ be the predicate "We are cousins" and $Q$ be the predicate "We are both
knaves."

Troll 1 then says:

$$ P \to Q $$

Troll 2 says:

$$ P \vee Q $$

We can use truth tables to actually explore all possibilities.

| $P$ | $Q$ | $P \to Q$ | $P \vee Q$ |
| --- | --- | --------- | ---------- |
| T   | T   | T         | T          |
| T   | F   | F         | T          |
| F   | T   | T         | T          |
| F   | F   | T         | F          |

In order for our tested conclusion, "Both trolls are knights" to be true, then
$Q$, "We are both knaves." must be false.

| $P$ | $Q$ | $P \to Q$ | $P \vee Q$ |
| --- | --- | --------- | ---------- |
| T   | F   | F         | T          |
| F   | F   | T         | F          |

Ah, but if we isolate for that here, we can see that at least one of our
premises is false, meaning that at least one of the trolls is lying, and
therefore it is not possible for both trolls to be knights.

2. Next you come upon three trolls, helpfully wearing name tags. They say:

Pat: "If either Quinn or I are knights, then so is Ryan."

Quinn: "Ryan is a knight, and if Pat is a knight, then so am I."

Ryan: "Quinn is a knave, but Pat and I share the same persuasion."

Create a truth table that includes all three statements. Then use the truth
table to determine the persuasion of each troll.

Let $P$ be "Pat is a knight", let "Q" be "Quinn is a knight", and let $R$ be
"Ryan is a knight."

Pat claims:

$$ (Q \vee P) \to R $$

Quinn claims:

$$ R \wedge (P \to Q) $$

Ryan claims:

$$ \neg Q \wedge (R \leftrightarrow P)$$

| $P$ | $Q$ | $R$ | $(Q \vee P)$ | $(P \to Q)$ | $\neg Q$ | $(R \leftrightarrow P)$ | $(Q \vee P) \to R$ | $R \wedge (P \to Q)$ | $\neg Q \wedge (R \leftrightarrow P)$ |
| --- | --- | --- | ------------ | ----------- | -------- | ----------------------- | ------------------ | -------------------- | ------------------------------------- |
| T   | T   | T   | T            | T           | F        | T                       | T                  | T                    | F                                     |
| T   | T   | F   | T            | T           | F        | F                       | F                  | F                    | F                                     |
| T   | F   | T   | T            | F           | T        | T                       | T                  | F                    | T                                     |
| T   | F   | F   | T            | F           | T        | F                       | F                  | F                    | F                                     |
| F   | T   | T   | T            | T           | F        | F                       | T                  | T                    | F                                     |
| F   | T   | F   | T            | T           | F        | T                       | F                  | F                    | F                                     |
| F   | F   | T   | F            | T           | T        | F                       | T                  | T                    | F                                     |
| F   | F   | F   | F            | T           | T        | T                       | T                  | F                    | T                                     |

Now we check each Premise $P$, $Q$, and $R$ as True and compare against whether
their respective claims are also true:

---

Pat:

$$ (Q \vee P) \to R $$

| $P$ | $Q$ | $R$ | $(Q \vee P)$ | $(P \to Q)$ | $\neg Q$ | $(R \leftrightarrow P)$ | $(Q \vee P) \to R$ | $R \wedge (P \to Q)$ | $\neg Q \wedge (R \leftrightarrow P)$ |
| --- | --- | --- | ------------ | ----------- | -------- | ----------------------- | ------------------ | -------------------- | ------------------------------------- |
| T   | T   | T   | T            | T           | F        | T                       | T                  | T                    | F                                     |
| T   | F   | T   | T            | F           | T        | T                       | T                  | F                    | T                                     |

In the first row:

The assertion Pat makes, $P$, is true, and his claim $(Q \vee P) \to R$ is also
true.

The assertion Quinn makes, $Q$, is true, and her claim $R \wedge (P \to R)$ is
true.

The assertion Ryan makes, $R$, is true, and his claim
$\neg Q \wedge (R \leftrightarrow)$ is false.

Because the validity of Ryan's assertion does not correspond with the validity
of his claim, this is not useful in determining the persuasion of each troll.

In the second row:

The assertion Pat makes, $P$, is true, and his claim $(Q \vee P) \to R$ is also
true.

The assertion Quinn makes, $Q$, is false, and her claim $R \wedge (P \to R)$ is
false.

The assertion Ryan makes, $R$, is true, and his claim
$\neg Q \wedge (R \leftrightarrow)$ is true.

This last row demonstrates the persuasion of each troll.

---

Quinn:

$$ R \wedge (P \to Q) $$

| $P$ | $Q$ | $R$ | $(Q \vee P)$ | $(P \to Q)$ | $\neg Q$ | $(R \leftrightarrow P)$ | $(Q \vee P) \to R$ | $R \wedge (P \to Q)$ | $\neg Q \wedge (R \leftrightarrow P)$ |
| --- | --- | --- | ------------ | ----------- | -------- | ----------------------- | ------------------ | -------------------- | ------------------------------------- |
| T   | T   | T   | T            | T           | F        | T                       | T                  | T                    | F                                     |
| F   | T   | T   | T            | T           | F        | F                       | T                  | T                    | F                                     |

In the first row:

The assertion Pat makes, $P$, is true, and his claim $(Q \vee P) \to R$ is also
true.

The assertion Quinn makes, $Q$, is true, and her claim $R \wedge (P \to R)$ is
true.

The assertion Ryan makes, $R$, is true, and his claim
$\neg Q \wedge (R \leftrightarrow)$ is false.

Because the validity of Ryan's assertion does not correspond with the validity
of his claim, this is not useful in determining the persuasion of each troll.

In the second row:

The assertion Pat makes, $P$, is false, and his claim $(Q \vee P) \to R$ is
true.

Because the validity of Pat's assertion does not correspond with the validity of
his claim, this is not useful in determining the persuasion of each troll.

---

Ryan:

$$ \neg Q \wedge (R \leftrightarrow P)$$

| $P$ | $Q$ | $R$ | $(Q \vee P)$ | $(P \to Q)$ | $\neg Q$ | $(R \leftrightarrow P)$ | $(Q \vee P) \to R$ | $R \wedge (P \to Q)$ | $\neg Q \wedge (R \leftrightarrow P)$ |
| --- | --- | --- | ------------ | ----------- | -------- | ----------------------- | ------------------ | -------------------- | ------------------------------------- |
| T   | F   | T   | T            | F           | T        | T                       | T                  | F                    | T                                     |

The assertion Pat makes, $P$, is true, and corresponds with the claim Pat makes
$(Q \vee P) \to R$, and is true. This matches.

The assertion that Quin makes, $Q$, is false, and corresponds with the claim
Quin makes $R \wedge (P \to Q)$.

The assertion that Ryan makes, $R$, is true, and corresponds with the claim Ryan
makes $\neg Q \wedge (R \leftrightarrow P)$.

This last row demonstrates the persuasion of each troll.

In conclusion, we can confidently say that Pat is a knight, Quinn is a knave,
and Ryan is a knight.

3.

Q: Consider the statement about a party, "If it's your birthday or there will be
cake, then there will be cake."

(a) Translate the above statement into symbols. Clearly state which statement is
$P$ and which is $Q$.

(b) Make a truth table for the statement.

\(c\) Assuming the statement is true, what (if anything) can you conclude if you
know there will be cake?

(d) Assuming the statement is true, what (if anything) can you conclude if you
know there will not be cake?

(e) Suppose you found out that the statement was a lie. What can you conclude?

A:

(a) Translate the above statement into symbols. Clearly state which statement is
$P$ and which is $Q$.

Let $P$ be "It's your birthday", and let $Q$ be "There will be cake."

So, in symbols, the given statement is:

$$ P \vee Q \to Q $$

(b) Make a truth table for the statement.

| $P$ | $Q$ | $P \vee Q$ | $P \vee Q \to Q$ |
| --- | --- | ---------- | ---------------- |
| T   | T   | T          | T                |
| T   | F   | T          | F                |
| F   | T   | T          | T                |
| F   | F   | F          | T                |

\(c\) Assuming the statement is true, what (if anything) can you conclude if you
know there will be cake?

| $P$ | $Q$ | $P \vee Q$ | $P \vee Q \to Q$ |
| --- | --- | ---------- | ---------------- |
| T   | T   | T          | T                |
| F   | T   | T          | T                |

I can conclude that there will be cake whether or not it's my birthday.

(d) Assuming the statement is true, what (if anything) can you conclude if you
know there will not be cake?

| $P$ | $Q$ | $P \vee Q$ | $P \vee Q \to Q$ |
| --- | --- | ---------- | ---------------- |
| F   | F   | F          | T                |

If I assume the statement $P \vee Q \to Q$ is true, and I know there will not be
cake $Q=F$, then I know it's not my birthday.

(e) Suppose you found out that the statement was a lie. What can you conclude?

| $P$ | $Q$ | $P \vee Q$ | $P \vee Q \to Q$ |
| --- | --- | ---------- | ---------------- |
| T   | F   | T          | F                |

I can conclude that it is my birthday and that there is no cake.

4.

Q: Geoff Poshingten is out at a fancy pizza joint and decides to order a
calzone. When the waiter asks what he would like in it, he replies, "I want
either pepperoni or sausage. Also, if I have sausage, then I must also include
quail. Oh, and if I have pepperoni or quail, then I must also have ricotta
cheese."

(a) Translate Geoff's order into logical symbols.

(b) The waiter knows that Geoff is either a liar or a truth-teller (so either
everything he says is false, or everything is true). Which is it?

\(c\) What, if anything, can the waiter conclude about the ingredients in
Geoff's desired calzone?

A:

(a) Translate Geoff's order into logical symbols.

Let $P$ be "Geoff has pepperoni." Let $S$ be "Geoff has sausage." Let $Q$ be
"Geoff has quail." Let $R$ be "Geoff has Ricotta Cheese."

"I want either pepperoni or sausage":

$$ P \vee S $$

"If I have sausage, then I must also include quail."

$$ S \to Q $$

"If I have pepperoni or quail, then I must also have ricotta cheese."

$$ (P \vee Q) \to R $$

(b) The waiter knows that Geoff is either a liar or a truth-teller (so either
everything he says is false, or everything is true). Which is it?

| $P$ | $S$ | $Q$ | $R | $P \vee S$ | $S \to Q$ | $P \vee Q$ | $(P \vee Q) \to R$ |
| --- | --- | --- | -- | ---------- | --------- | ---------- | ------------------ |
| T   | T   | T   | T  | T          | T         | T          | T                  |
| T   | T   | T   | F  | T          | T         | T          | F                  |
| T   | T   | F   | T  | T          | F         | T          | T                  |
| T   | T   | F   | F  | T          | F         | T          | F                  |
| T   | F   | T   | T  | T          | T         | T          | T                  |
| T   | F   | T   | F  | T          | T         | T          | F                  |
| T   | F   | F   | T  | T          | T         | T          | T                  |
| T   | F   | F   | F  | T          | T         | T          | F                  |
| F   | T   | T   | T  | T          | T         | T          | T                  |
| F   | T   | T   | F  | T          | T         | T          | F                  |
| F   | T   | F   | T  | T          | F         | F          | T                  |
| F   | T   | F   | F  | T          | F         | F          | T                  |
| F   | F   | T   | T  | F          | T         | T          | T                  |
| F   | F   | T   | F  | F          | T         | T          | F                  |
| F   | F   | F   | T  | F          | T         | F          | T                  |
| F   | F   | F   | F  | F          | T         | F          | T                  |

Let's now filter where all the claims are true, $P \vee S$, $S \to Q$, and
$(P \vee Q) \to R$:

| $P$ | $S$ | $Q$ | $R | $P \vee S$ | $S \to Q$ | $P \vee Q$ | $(P \vee Q) \to R$ |
| --- | --- | --- | -- | ---------- | --------- | ---------- | ------------------ |
| T   | T   | T   | T  | T          | T         | T          | T                  |

Let's now filter where all the claims are false, $P \vee S$, $S \to Q$, and
$(P \vee Q) \to R$:

| $P$ | $S$ | $Q$ | $R | $P \vee S$ | $S \to Q$ | $P \vee Q$ | $(P \vee Q) \to R$ |
| --- | --- | --- | -- | ---------- | --------- | ---------- | ------------------ |
|     |     |     |    |            |           |            |                    |

And there are no rows where all three claims of Geoff's are F (i.e., he is
lying). So everything he says is true. Geoff is a truth-teller.

\(c\) What, if anything, can the waiter conclude about the ingredients in
Geoff's desired calzone?

Since we've concluded already that Geoff is a truth-teller, that means
everything he says is true, let's examine all possible claims where Geoff's
claims are true:

So, breaking it down:

$P \vee S$: Geoff is getting either Pepperoni or Sausage or both.

$S \to Q$ If Geoff has Sausage, he also has Quail.

$P \vee Q$: Geoff is getting either pepperoni or quail or both.

$(P \vee Q) \to R$: If Geoff gets either pepperoni or Quail or both, he has
Ricotta cheese.

| $P$ | $S$ | $Q$ | $R | $P \vee S$ | $S \to Q$ | $(P \vee Q) \to R$ |
| --- | --- | --- | -- | ---------- | --------- | ------------------ |
| T   | T   | T   | T  | T          | T         | T                  |
| T   | F   | T   | T  | T          | T         | T                  |
| T   | F   | F   | T  | T          | T         | T                  |
| F   | T   | T   | T  | T          | T         | T                  |

The only thing that is consistent is that Geoff gets Ricotta cheese. We are
unable to determine which other ingredients that Geoff will include in his
Calzone.

5.

Q: Determine whether the following two statements are logically equivalent:
$\neg (P \to Q)$ and $P \wedge \neg Q$. Explain how you know you are correct.

A:

We can use a truth table:

| $P$ | $Q$ | $(P \to Q)$ | $\neg (P \to Q)$ | $\neg Q$ | $P \wedge \neg Q$ |
| --- | --- | ----------- | ---------------- | -------- | ----------------- |
| T   | T   | T           | F                | F        | F                 |
| T   | F   | F           | T                | T        | T                 |
| F   | T   | T           | F                | F        | F                 |
| F   | F   | T           | F                | T        | F                 |

And then we just compare the two statement's rows:

| $\neg (P \to Q)$ | $P \wedge \neg Q$ |
| ---------------- | ----------------- |
| F                | F                 |
| T                | T                 |
| F                | F                 |
| F                | F                 |

This is also the same problem presented in Example 1.3.8, which asks us to prove
logical equivalency without truth tables.

Let's first take our first statement:

$$ \neg (P \to Q) $$

Recall that implications are also disjunctions:

$$ P \to Q \equiv \neg P \vee Q $$

So we can apply this to our first statement:

$$ \neg (\neg P \vee Q) $$

And De Morgan's law tells us we can "distribute" a negation as long as we change
the disjunction to a conjunction:

$$ \neg\neg P \wedge \neg Q $$

And then we get rid of the double negation:

$$ P \wedge \neg Q $$

And this is our second statement. We have proven that these two statements are
equivalent through this transformation steps as well:

$$ \neg (P \to Q) \equiv P \wedge \neg Q $$

6.

Q: Simplify the following statements (so that negation only appears right before
variables).

(a) $\neg (P \to \neg Q)$.

(b) $(\neg P \vee \neg Q) \to \neg(\neg Q \wedge R)$.

\(c\) $\neg((P \to \neg Q) \vee (R \wedge \neg R))$.

(d) It is false that if Sam is not a man then Chris is a woman, and that Chris
is not a woman.

A:

(a) $\neg (P \to \neg Q)$.

$P \to \neg Q$ is false when $P$ is true and $Q$ is false. We can rewrite this
as:

$$ P \to \neg Q \equiv \neg(P \wedge \neg Q) $$

This makes our original statement:

$$ \neg (P \to \neg Q) \equiv \neg (\neg(P \wedge \neg Q)) $$

Let's then use De Morgan's Law:

$$  \neg (\neg P \vee \neg\neg Q) $$

$$  \neg (\neg P \vee Q) $$

And again with De Morgan's Law:

$$  \neg\neg P \wedge \neg Q $$

$$  \boxed{P \wedge \neg Q} $$

(b) $(\neg P \vee \neg Q) \to \neg(\neg Q \wedge R)$.

$$ (\neg P \vee \neg Q) \to (\neg\neg Q \vee \neg R) $$

$$ (\neg P \vee \neg Q) \to (Q \vee \neg R) $$

\(c\) $\neg((P \to \neg Q) \vee (R \wedge \neg R))$.

$P \to \neg Q$ is false only when $P$ is true and $Q$ is true.

$$ \neg(\neg(P \wedge Q) \vee (R \wedge \neg R)) $$

$$ \neg\neg(P \wedge Q) \wedge \neg(R \wedge \neg R) $$

$$ (P \wedge Q) \wedge (\neg R \vee R) $$

This looks finished, but we can go one step forward with the second operator:

$$ \neg R \vee R \equiv T $$

This will always be true.

$$ (P \wedge Q) \wedge T $$

Because forming a conjunction with an always true statement will always depend
on the ambiguous statement (the not always true statement), we can simply drop
the always true:

$$ \boxed{P \wedge Q} $$

(d) It is false that if Sam is not a man then Chris is a woman, and that Chris
is not a woman.

Let $S$ be "Sam is a man" and $C$ be "Chris is a woman".

$$ \neg (\neg S \to C) \wedge \neg C $$

Note the wording here is specific, the "It is false" applies only to the first
part of the problem statement sentence, not the second

$\neg S \to C$ is false only if $S$ is false and $C$ is false.

$$ \neg (\neg S \wedge \neg C) \wedge \neg C $$

$$ (S \vee C) \wedge \neg C $$

We need to consider both "or" cases:

$$ ((S \wedge C) \vee (S \wedge \neg C)) \wedge \neg C $$

$$ (S \wedge (C \vee \neg C)) \wedge \neg C $$

$$ (S \wedge T) \wedge \neg C $$

$$ \boxed{S \wedge \neg C} $$

7.

Q: Use De Morgan's Laws and any other logical equivalence facts you know to
simplify the following statements. Show all your steps. Your final statements
should have negations only appear directly next to the sentence variables or
predicates ($P$, $Q$, $E(x)$, etc.), and no double negations. It would be a good
idea to use only conjunctions, disjuctions, and negations.

(a) $\neg((\neg P \wedge Q) \vee \neg (R \vee \neg S))$.

$$ \neg((\neg P \wedge Q) \vee \neg (R \vee \neg S)) $$

Let's "distribute" the outside negation first:

$$ \neg(\neg P \wedge Q) \wedge \neg\neg (R \vee \neg S) $$

Get rid of the double negative on the second "term":

$$ \neg(\neg P \wedge Q) \wedge (R \vee \neg S) $$

And "distribute" the negation on the first "term":

$$ (\neg\neg P \vee \neg Q) \wedge (R \vee \neg S) $$

And again, get rid of the double negative:

$$ \boxed{(P \vee \neg Q) \wedge (R \vee \neg S)} $$

(b) $\neg ((\neg P \to \neg Q) \wedge (\neg Q \to R))$ (careful with the
implications)

$$ \neg ((\neg P \to \neg Q) \wedge (\neg Q \to R)) $$

First let's "distribute" the outside negation:

$$ \neg(\neg P \to \neg Q) \vee \neg(\neg Q \to R) $$

Now apply "Implications are Disjunctions":

$$ \neg(P \vee \neg Q) \vee \neg(Q \vee R) $$

Note the reason it takes this form is that implications are disjunctions only
negates the antecedent (the first term of an if/then statement, not the
consequent). Now we can apply De Morgan's Laws again to each "term":

$$ (\neg P \wedge Q) \vee (\neg Q \wedge \neg R) $$

\(c\) For both parts above, verify your answers are correct using truth tables.
That is, use a truth table to check that the given statement and your proposed
simplification are actually logically equivalent.

For part (a), we start at: $\neg((\neg P \wedge Q) \vee \neg (R \vee \neg S))$,
and we end at $(P \vee \neg Q) \wedge (R \vee \neg S)$:

| $P$ | $Q$ | $R$ | $S$ | $\neg((\neg P \wedge Q) \vee \neg(R \vee \neg S))$ | $(P \vee \neg Q) \wedge (R \vee \neg S)$ |
| --- | --- | --- | --- | -------------------------------------------------- | ---------------------------------------- |
| T   | T   | T   | T   | T                                                  | T                                        |
| T   | T   | T   | F   | T                                                  | T                                        |
| T   | T   | F   | T   | F                                                  | F                                        |
| T   | T   | F   | F   | T                                                  | T                                        |
| T   | F   | T   | T   | T                                                  | T                                        |
| T   | F   | T   | F   | T                                                  | T                                        |
| T   | F   | F   | T   | F                                                  | F                                        |
| T   | F   | F   | F   | F                                                  | F                                        |
| F   | T   | T   | T   | F                                                  | F                                        |
| F   | T   | T   | F   | F                                                  | F                                        |
| F   | T   | F   | T   | F                                                  | F                                        |
| F   | T   | F   | F   | F                                                  | F                                        |
| F   | F   | T   | T   | T                                                  | T                                        |
| F   | F   | T   | F   | T                                                  | T                                        |
| F   | F   | F   | T   | F                                                  | F                                        |
| F   | F   | F   | F   | T                                                  | T                                        |

These two statements are logically equivalent, as their truth tables, when
evaluated, produce exactly the same results in all cases. It is reasonable to
conclude that:

$$ \neg((\neg P \wedge Q) \vee \neg(R \vee \neg S)) \equiv (P \vee \neg Q) \wedge (R \vee \neg S) $$

8.

Q: Consider the statement, "If a number is triangular or square, then it is not
prime"

(a) Make a truth table for the statement $(T \vee S) \to \neg P$.

(b) If you believed the statement was _false_, what properties would a
counterexample need to possess? Explain by referencing your truth table.

\(c\) If the statement were true, what could you conclude about the number 5657,
which is definitely prime? Again, explain using the truth table.

A:

(a) Make a truth table for the statement $(T \vee S) \to \neg P$.

| $T$ | $S$ | $P$ | $(T \vee S)$ | $\neg P$ | $(T \vee S) \to \neg P$ |
| --- | --- | --- | ------------ | -------- | ----------------------- |
| T   | T   | T   | T            | F        | F                       |
| T   | T   | F   | T            | T        | T                       |
| T   | F   | T   | T            | F        | F                       |
| T   | F   | F   | T            | T        | T                       |
| F   | T   | T   | T            | F        | F                       |
| F   | T   | F   | T            | T        | T                       |
| F   | F   | T   | F            | F        | T                       |
| F   | F   | F   | F            | T        | T                       |

(b) If you believed the statement was _false_, what properties would a
counterexample need to possess? Explain by referencing your truth table.

The only examples where the statement $(T \vee S) \to \neg P$ are false are
indicated by these rows from the truth table:

| $T$ | $S$ | $P$ | $(T \vee S)$ | $\neg P$ | $(T \vee S) \to \neg P$ |
| --- | --- | --- | ------------ | -------- | ----------------------- |
| T   | T   | T   | T            | F        | F                       |
| T   | F   | T   | T            | F        | F                       |
| F   | T   | T   | T            | F        | F                       |

From the truth table, $(T \vee S) \to \neg P$ is false exactly when:

- $T \vee S = T$ (the number is triangular or square, or both), and

- $\neg P = F$, meaning $P = T$ (the number is prime).

So a counterexample must be a prime number that is either triangular, square, or
both.

In other words, the number must satisfy:

$$ P = T \quad \text{ and } \quad (T \vee S) = T $$

Equivalently, the number is prime but also has at least one of the properties
"triangular" or "square."

\(c\) If the statement were true, what could you conclude about the number 5657,
which is definitely prime? Again, explain using the truth table.

Let us express this as $P(5657) = T$, and also the statement itself is true,
$(T \vee S) \to \neg P = T$.

If we isolate our table where $P = T$ and $(T \vee S) \to \neg P = T$, then we
get:

| $T$ | $S$ | $P$ | $(T \vee S)$ | $\neg P$ | $(T \vee S) \to \neg P$ |
| --- | --- | --- | ------------ | -------- | ----------------------- |
| F   | F   | T   | F            | F        | T                       |

This implies that since 5657 is prime, and the statement is true, that the
hypothesis $(T \vee S)$ in this case is false, while the conclusion, $\neg P$ is
true. Therefore, 5657 is neither triangular nor square.

9.

Q: Tommy Flanagan was telling you what he ate yesterday afternoon. He tells you,
"I had either popcorn or raisins. Also, if I had cucumber sandwiches, then I had
soda. But I didn't drink soda or tea." Of course, you know that Tommy is the
world's worst liar, and everything he says is false. What did Tommy eat?

Justify your answer by writing all of Tommy's statements using sentence
variables ($P$, $Q$, $R$, $S$, $T$), taking their negations, and using these to
deduce what Tommy actually ate.

A:

Let the following variables represent the following statements:

$P$: "Tommy had popcorn."

$Q$: "Tommy had raisins."

$R$: "Tommy had cucumber sandwiches."

$S$: "Tommy had soda."

$T$: "Tommy had tea."

Breaking this down for later use, we get:

$(P \vee Q)$: "Tommy had either popcorn or raisins."

$R \to S$ "If Tommy had cucumber sandwiches, then he had soda."

$\neg(S \vee T)$: "Tommy doesn't drink soda or tea."

This evaluates to:

$$ (P \vee Q) \wedge (R \to S) \wedge \neg(S \vee T) $$

And lastly we know Tommy is a liar, so we negate the entire statement:

$$ \neg((P \vee Q) \wedge (R \to S) \wedge \neg(S \vee T)) $$

Let's use De Morgan's Laws and Implications are Disjunctions and negations to
see if we can't express this in a way that we can find out what Tommy ate.

First, implications are disjunctions for the "middle term":

$$ \neg((P \vee Q) \wedge (\neg R \vee S) \wedge \neg(S \vee T)) $$

Let's apply De Morgan's Laws to the "last term":

$$ \neg((P \vee Q) \wedge (\neg R \vee S) \wedge (\neg S \wedge \neg T)) $$

And De Morgan's Laws again on the entire statement:

$$ \neg(P \vee Q) \vee \neg(\neg R \vee S) \vee \neg(\neg S \wedge \neg T) $$

$$ (\neg P \wedge \neg Q) \vee (R \wedge \neg S) \vee (S \vee T) $$

Ultimately now we have to prove that this statement will always be false, since
Tommy is a liar.

$$ (\neg P \wedge \neg Q) \vee (R \wedge \neg S) \vee (S \vee T) = F $$

Since these are three separate atomic statements joined by disjunctions, this
means that each individual statement must be false.

$$ (\neg P \wedge \neg Q) = F $$

So this means that Tommy did not have popcorn or raisins, but he might have had
one or the other.

$$ (R \wedge \neg S) = F $$

This means that Tommy did not have cucumber sandwiches, but he did have a soda,
or he did have cucumber sandwiches and did not have a soda.

$$ (S \vee T) = F $$

This means that Tommy didn't drink Soda or Tea. He didn't drink anything. This
is the most definitive statement. Knowing this, we can further refine our
evaluation of the other two statements.

$$ (R \wedge \neg S) = F $$

Since we know that $\neg S = T$, this means that $R = F$. Tommy did not eat
cucumber sandwiches.

$$ (\neg P \wedge \neg Q) = F $$

Here we know the least, we know that Tommy either had popcorn or raisins, but he
had at least one of them.

In conclusion, we know the following:

- Tommy did not drink soda or tea
- Tommy did not eat cucumber sandwiches
- Tommy either had either popcorn or raisins or both.

10. Can you chain implications together? That is, if $P \to Q$ and $Q \to R$,
    does that mean the $P \to R$? Prove that the following is a valid deduction
    rule:

$$
P \to Q \\
Q \to R \\
\overline{\therefore P \to R}
$$

This is solved best when using a truth table:

| $P$ | $Q$ | $R$ | $P \to Q$ | $Q \to R$ | $P \to R$ |
| --- | --- | --- | --------- | --------- | --------- |
| T   | T   | T   | T         | T         | T         |
| T   | T   | F   | T         | F         | F         |
| T   | F   | T   | F         | T         | T         |
| T   | F   | F   | F         | T         | F         |
| F   | T   | T   | T         | T         | T         |
| F   | T   | F   | T         | F         | T         |
| F   | F   | T   | T         | T         | T         |
| F   | F   | F   | T         | T         | T         |

We're only concerned where our antecedents are true, so let's highlight which
ones have antecedents that are both true, wherever this is the case, we will
also highlight the conclusion's true/false value and compare it to the
antecedents.

| $P$ | $Q$ | $R$ | $P \to Q$ | $Q \to R$ | $P \to R$ |
| --- | --- | --- | --------- | --------- | --------- |
| T   | T   | T   | **T**     | **T**     | **T**     |
| T   | T   | F   | T         | F         | F         |
| T   | F   | T   | F         | T         | T         |
| T   | F   | F   | F         | T         | F         |
| F   | T   | T   | **T**     | **T**     | **T**     |
| F   | T   | F   | T         | F         | T         |
| F   | F   | T   | **T**     | **T**     | **T**     |
| F   | F   | F   | **T**     | **T**     | **T**     |

And as we can see, when we do this, the consequent is also always true,
therefore this is a valid deduction rule.

11.

Q: Suppose $P$ and $Q$ are (possibly molecular) propositional statements. Prove
that $P$ and $Q$ are logically equivalent if and only if $P \leftrightarrow Q$
is a tautology.

A:

Let's break this down with the standard "if and only if" truth table:

| $P$ | $Q$ | $P \leftrightarrow Q$ |
| --- | --- | --------------------- |
| T   | T   | T                     |
| T   | F   | F                     |
| F   | T   | F                     |
| F   | F   | T                     |

For $P$ and $Q$ to be logically equivalent, both of the following statements
must be true:

$$ P \to Q $$

And

$$ Q \to P $$

This evaluates to:

$$ (P \to Q) \wedge (Q \to P) $$

Let's expand our truth table to include these statements as well so we can
further evaluate whether or not $P \leftrightarrow Q$ is a tautology:

| $P$ | $Q$ | $P \to Q$ | $Q \to P$ | $(P \to Q) \wedge (Q \to P)$ | $P \leftrightarrow Q$ |
| --- | --- | --------- | --------- | ---------------------------- | --------------------- |
| T   | T   | T         | T         | T                            | T                     |
| T   | F   | F         | T         | F                            | F                     |
| F   | T   | T         | F         | F                            | F                     |
| F   | F   | T         | T         | T                            | T                     |

As seen in the last two columns, $(P \to Q) \wedge (Q \to P)$ and
$P \leftrightarrow Q$ have identical truth values in every row. This means they
are logically equivalent. Since $P \leftrightarrow Q$ is true exactly when $P$
and $Q$ have the same truth value, it follows that it is true in all cases where
logical equivalence holds, and thus characterizes a tautology condition.

12.

Q: Suppose $P_1, P_2, \dots , P_n$ and $Q$ are (possibly molecular)
propositional statements. Suppose further that

$$
P_1 \\
P_2 \\
\vdots \\
P_n \\
\overline{\therefore Q}
$$

is a valid deduction rule. Prove that the statement

$$ (P_1 \wedge P_2 \wedge \dots \wedge P_n) \to Q $$

is a tautology.

A:

A deduction rule is valid where there are no premises that result in a false
conclusion. Since we know that:

$$
P_1 \\
P_2 \\
\vdots \\
P_n \\
\overline{\therefore Q}
$$

is a valid deduction rule, we also know then that there is no case where all
$P_1 \dots P_n$ are true and $Q$ is false. The implication is that
$(P_1 \wedge \dots \wedge P_n) \to Q$ is always true, therefore it is a
tautology.

$$ (P_1 \wedge \dots \wedge P_n) \to Q $$

13.

Q: Consider the statements below. Translate each into symbols, using the
predicate $F(x, y)$ for "person $x$ can be fooled at any time $y$." Decide
whether any of the statements are equivalent to each other, or whether any imply
any others, in this context or in general.

(a) You can fool some people all of the time.

(b) You can fool everyone some of the time.

\(c\) You can always fool some people.

(d) Sometimes you can fool everyone.

A:

Let's first just translate each of these into symbols

(a) You can fool some people all of the time.

$$ \exists x \forall y F(x, y) $$

(b) You can fool everyone some of the time.

$$ \forall x \exists y F(x, y) $$

\(c\) You can always fool some people.

$$ \forall y \exists x F(x, y) $$

(d) Sometimes you can fool everyone.

$$ \exists y \forall x F(x, y) $$

None of these statements are logically equivalent to each other. Equivalencies
with quantifiers always involve some negation of the quantifier(s) or the
antecedent(s). There are no negations here and so none of them are logically
equivalent. However yes, some do imply others.

(a) does imply \(c\):

$$ \exists x \forall y F(x, y) \to \forall y \exists x F(x, y) $$

"If there exists some person $x$ for all times $y$ for which that person is
fooled, then for all times $y$, there is at least one person $x$ who is fooled."

and (d) does imply (b):

$$ \exists y \forall x F(x, y) \to forall x \exists y F(x, y) $$

"If there exists some time $y$ for all people $x$ where all people are fooled,
then for all people $x$ there exists at least one time $y$ where all people are
fooled."

14.

Q: Suppose $P(x)$ is some predicate for which the statement $\forall x P(x)$ is
true. Is it also the case that $\exists x P(x)$ is true? In other words, is the
statement $\forall x P(x) \to \exists x P(x)$ always true? Is the converse
always true? Assume the domain of discourse is non-empty.

A:

Let's break this down:

Suppose $P(x)$ is some predicate for which the statement $\forall x P(x)$ is
true. Is it also the case that $\exists x P(x)$ is true?

Is this true?:

$$ \forall x P(x) \to \exists x P(x) $$

Since we know that $\forall x P(x)$ is true for all $x$, $P(x)$ holds for every
element of the domain. Because we also know that the domain of discourse is not
empty, we can choose some element $a$ for which $P(a)$ is true. Therefore,
$\exists x P(x)$ is true.

15.

Q: Simplifying negations will be especially useful when we try to prove a
statement by considering what would happen if it were false. For each statement
below, write the _negation_ of the statement as simply as possible. Don't just
say, "It is false that..."

(a) Every number is either even or odd.

(b) There is a sequence that is both arithmetic and geometric.

\(c\) For all numbers, $n$, if $n$ is prime, then $n + 3$ is not prime.

A:

(a) Every number is either even or odd.

Let's start by writing the statement as is:

Let $E(x)$ be "The number is even" and $O(x)$ be "the number is odd."

So this original statement is:

$$ \forall x (E(x) \vee O(x)) $$

Then we apply a negation over the whole statement:

$$ \neg\forall x (E(x) \vee O(x)) $$

From the section on Quantifiers and negation we know that:

$\neg \forall x P(x)$ is equivalent to $\exists x \neg P(x)$.

$\neg \exists x P(x)$ is equivalent to $\forall x \neg P(x)$.

So we can write this as logically equivalent to:

$$ \neg\forall x (E(x) \vee O(x)) \equiv \exists x \neg (E(x) \vee O(x)) $$

Taking this equivalency we can rewrite it using De Morgan's Laws:

$$ \exists x \neg (E(x) \vee O(x)) $$

$$ \exists x (\neg E(x) \wedge \neg O(x)) $$

Which says:

"There exists at least one number $x$ which is neither even nor odd."

(b) There is a sequence that is both arithmetic and geometric.

Let $x$ be some sequence, and let $A(x)$ be "The sequence is arithmetic", and
$G(x)$ be "The sequence is geometric."

So our original statement reads as:

$$ \exists x (A(x) \wedge G(x)) $$

Now we negate it:

$$ \neg\exists x (A(x) \wedge G(x)) $$

Again, we look to the section on Quantifiers and negation:

$\neg \forall x P(x)$ is equivalent to $\exists x \neg P(x)$.

$\neg \exists x P(x)$ is equivalent to $\forall x \neg P(x)$.

$$ \neg\exists x (A(x) \wedge G(x)) \equiv \forall x \neg (A(x) \wedge G(x)) $$

And apply De Morgan's Laws:

$$ \forall x \neg (A(x) \wedge G(x)) $$

$$ \forall x (\neg A(x) \vee \neg G(x)) $$

Which says:

"All sequences $x$ are either not arithmetic or not geometric."

\(c\) For all numbers, $n$, if $n$ is prime, then $n + 3$ is not prime.

Let $P(n)$ be "The number $n$ is prime".

So the original statement is:

$$ \forall n (P(n) \to \neg P(n + 3)) $$

Let's write this implication as a disjunction:

$$ \forall n (\neg P(n) \vee \neg P(n + 3)) $$

Again, we look to the section on Quantifiers and negation:

$\neg \forall x P(x)$ is equivalent to $\exists x \neg P(x)$.

$\neg \exists x P(x)$ is equivalent to $\forall x \neg P(x)$.

$$ \forall n (\neg P(n) \vee \neg P(n + 3)) \equiv \exists n \neg(\neg P(n) \vee \neg P(n + 3)) $$

$$ \exists n \neg(\neg P(n) \vee \neg P(n + 3)) $$

Now we use De Morgan's Laws:

$$ \exists n (P(n) \wedge P(n + 3)) $$

Now this says:

"There exists some number $n$ for which $n$ is prime and $n + 3$ is prime."

16.

Q: We can simplify statements in predicate logic using our rules for passing
negations over quantifiers before applying logical equivalence to the "inside"
propositional part. Simplify the statements below (so negation appears only
directly next to predicates).

(a) $\neg \exists x \forall y (\neg O(x) \vee E(y))$.

(b)
$\neg \forall x \neg \forall y \neg(x < y \wedge \exists z (x < z \vee y < z))$.

\(c\) There is a number $n$ for which no other number is less than or equal to
$n$.

(d) It is false that for every number $n$ there are two other numbers which $n$
is between.

A:

Each of these will likely use Quantifiers and negation:

$\neg \forall x P(x)$ is equivalent to $\exists x \neg P(x)$.

$\neg \exists x P(x)$ is equivalent to $\forall x \neg P(x)$.

(a) $\neg \exists x \forall y (\neg O(x) \vee E(y))$.

$$ \neg \exists x \forall y (\neg O(x) \vee E(y)) $$

$$ \forall x \neg \forall y (\neg O(x) \vee E(y)) $$

$$ \forall x \exists y \neg(\neg O(x) \vee E(y)) $$

Then use De Morgan's Laws:

$$ \forall x \exists y (O(x) \wedge \neg E(y)) $$

(b)
$\neg \forall x \neg \forall y \neg(x < y \wedge \exists z (x < z \vee y < z))$.

$$ \neg \forall x \neg \forall y \neg(x < y \wedge \exists z (x < z \vee y < z)) $$

$$ \exists x \neg\neg \forall y \neg(x < y \wedge \exists z (x < z \vee y < z)) $$

$$ \exists x \forall y \neg(x < y \wedge \exists z (x < z \vee y < z)) $$

$$ \exists x \forall y (\neg(x < y) \vee \neg\exists z (x < z \vee y < z)) $$

$$ \exists x \forall y ((x \geq y) \vee \forall z \neg(x < z \vee y < z)) $$

$$ \exists x \forall y ((x \geq y) \vee \forall z (\neg(x < z) \wedge \neg(y < z))) $$

$$ \exists x \forall y ((x \geq y) \vee \forall z ((x \geq z) \wedge (y \geq z))) $$

\(c\) There is a number $n$ for which no other number is less than or equal to
$n$.

Let's first translate this:

$$ \exists n \neg\exists y (y \leq n) $$

Now let's simplify:

$$ \exists n \forall y \neg(y \leq n) $$

$$ \exists n \forall y (y > n) $$

(d) It is false that for every number $n$ there are two other numbers which $n$
is between.

Let's first translate this:

$$ \neg \forall n \exists x \exists y (x < n < y) $$

Now let's simplify:

$$ \exists n \neg\exists x \exists y (x < n < y) $$

$$ \exists n \forall x \neg\exists y (x < n < y) $$

$$ \exists n \forall x \forall y \neg(x < n < y) $$

In order to further simplify, it is best that we express $x < n < y$ as
$x < n \wedge n < y$:

$$ \exists n \forall x \forall y \neg(x < n \wedge n < y) $$

Now we can apply De Morgan's Laws:

$$ \exists n \forall x \forall y (\neg(x < n) \vee \neg(n < y)) $$

$$ \exists n \forall x \forall y ((x \geq n) \vee (n \geq y)) $$

17.

Q: Simplify the statements below to the point that negation symbols occur only
directly next to predicates.

(a) $\neg \forall x \forall y (x < y \vee y < x)$.

(b) $\neg (\exists x P(x) \to \forall y P(y))$.

A:

(a) $\neg \forall x \forall y (x < y \vee y < x)$.

$$ \neg \forall x \forall y (x < y \vee y < x) $$

$$ \exists x \neg\forall y (x < y \vee y < x) $$

$$ \exists x \exists y \neg(x < y \vee y < x) $$

$$ \exists x \exists y (\neg(x < y) \wedge \neg(y < x)) $$

$$ \exists x \exists y ((x \geq y) \wedge (y \geq x)) $$

(b) $\neg (\exists x P(x) \to \forall y P(y))$.

$$ \neg (\exists x P(x) \to \forall y P(y)) $$

Recall that implications are disjunctions:

$$ P \to Q \equiv \neg P \vee Q $$

So we can express our original statement as:

$$ \neg (\neg \exists x P(x) \vee \forall y P(y)) $$

Now use De Morgan's Laws:

$$ \exists x P(x) \wedge \neg \forall y P(y) $$

$$ \exists x P(x) \wedge \exists y \neg P(y) $$
