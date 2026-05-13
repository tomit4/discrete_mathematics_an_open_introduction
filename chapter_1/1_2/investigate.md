# Investigate!

Q: Little Timmy's Mom tells him, "If you don't eat all your broccoli, then you
will not get any ice cream." Of course, Timmy loves his ice cream, so he quickly
eats all his broccoli (which actually tastes pretty good).

After dinner, when Timmy asks for his ice cream, he is told no! Does Timmy have
a right to be upset? Why or why not?

A: Well, probably, but in the context of this class, I'm guessning no?

Let's think about this logically:

Let $P$ be the predicate "If you don't eat all your broccoli", and let $Q$ be
the conclusion "you will not get any ice cream."

This is expressed as:

$$ P \to Q $$

If we consult our truth tables from the last section, we have:

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |

But remember that Timmy did eat his broccoli, so that is actually $\neg P$.

| $P$ | $\neg P$ |
| --- | -------- |
| T   | F        |
| F   | T        |

This changes our if/then truth table:

| $\neg P$ | $Q$ | $P \to Q$ |
| -------- | --- | --------- |
| F        | T   | T         |
| F        | F   | F         |
| T        | T   | T         |
| T        | F   | T         |

Of note is the last three columns. The first of which shows that definitively,
Timmy's Mom is correct, if Timmy doesn't eat his broccoli, he will definitely
not get any ice cream:

| $\neg P$ | $Q$ | $P \to Q$ |
| -------- | --- | --------- |
| F        | F   | F         |

But notice the last two columns, where "If you eat all your broccoli" is true:

| $\neg P$ | $Q$ | $P \to Q$ |
| -------- | --- | --------- |
| T        | T   | T         |
| T        | F   | T         |

This equates to The mom explicitly saying "If you do eat your broccoli, you may
or may not get ice cream." Which is true, she never explicitly said that, lol.
But hey, Timmy's Mom, come on man!!
