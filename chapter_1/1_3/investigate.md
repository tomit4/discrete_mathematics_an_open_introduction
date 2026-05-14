# Investigate!

Holmes always wears one of the two vests he owns: one tweed and one mint green.
He always wears either the green vest or red shoes. Whenever he wears a purple
shirt and the green vest, he chooses to not wear a bow tie. He never wears the
green vest unless he is also wearing either a purple shirt or red shoes.
Whenever he wears red shoes, he also wears a purple shirt. Today, Holmes wore a
bow tie. What else did he wear?

## Try it 1.3.1

Spend a few minutes thinking about the _Investigate!_ question above. Of the six
statements in the puzzle, only one is atomic. Use this atomic statement and one
other statement to deduce a new statement about what Holmes might (or might not)
be wearing. Explain why you think your new statement is true.

**Hint**

The atomic statement is, "Holmes wore a bow tie." Only one of the molecular
statement has this as one of its atoms.

A:

Let $B$ be "Holmes wears a bow tie." Also, let' $P$ be "Holmes wears a purple
shirt" and $G$ be "Holmes wears a green vest".

Based off the molecular statement:

"Whenever he wears a purple shirt and the green vest, he chooses not to wear a
bow tie."

We can write this as:

$$ (P \wedge G) \to \neg B $$

But we know that $B$ is true from the problem statement, which means that Holmes
is not wearing a purple shirt and the green vest:

$$ \neg (P \wedge G) $$

Let's now write out the other statements. Let $R$ be "Holmes wears the red
shoes." We know from the problem statement that "He always wears either the
green vest or red shoes." This is written as:

$$ G \vee R $$

Let $T$ be "Holmes wears the tweed vest." We know from the problem statement
that "Holmes always wears one of the two vests he owns: one tweed and one mint
green." This is written as:

$$ T \vee G $$

"He never wears the green vest unless he is also wearing either a purple shirt
or red shoes.":

$$ G \to (P \vee R) $$

"Whenever he wears red shoes, he also wears a purple shirt."

$$ R \to P $$

This gives us everything we need, let's investigate what we know, and track back
through the problem to find out what Holmes is wearing.

$$ B \to \neg (P \wedge G) $$

While Holmes could be wearing either the purple shirt or the green vest, he
cannot wear them together. Let's assume he's wearing the green vest:

$$ G \to (P \vee R) $$

So he can't wear the purple shirt, but he can wear the red shoes.

$$ R \to P $$

Ah, that doesn't work, whenever Holmes wears the red shoes he also wears a
purple shirt. Therefore Holmes cannot be wearing the green vest.

$$ \neg G $$

So, now we consider "He always wears either the green vest or red shoes."

$$ G \vee R $$

Since we know that Holmes isn't wearing the green vest, therefore he must be
wearing the red shoes:

$$ R $$

And if he's wearing the red shoes, he is also wearing a purple shirt:

$$ R \to P $$

We also know that Holmes always either wears one of the two vests, the tweed or
the mint green.

$$ T \vee G $$

Since we know he's not wearing the green vest, he must be wearing the tweed
vest.

So Holmes is wearing a tweed vest, a bow tie, a purple shirt, and red shoes.
