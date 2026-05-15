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
