# Practice Problems

1.

Q: Arrange some of the statements below to form a correct proof of the following
statement: "For any integer $n$, if $n$ is even, then $7n$ is even."

- Let $n$ be an arbitrary integer, and assume $7n$ is even.

- Let $n$ be an arbitrary integer, and assume $7n$ is odd.

- Since $7$ is odd and the product of an odd number and an odd number is odd,

- Since an even number divided by $7$ must be odd,

- $n$ must be odd.

- $7n$ must be odd.

- Let $n$ be an arbitrary integer, and assume $n$ is even.

- Since the product of any number with an even number is even,

- $7n$ must be even.

A:

Let's establish the antecedent and consequent here.

$P(n)$ is "$n$ is even"

$Q(n)$ is "$7n$ is even"

$$ P(n) \to Q(n) $$

In a direct proof, we start with "assume the antecedent" and we end with
"therefore the consequent".

Proof by direct proof:

- Let $n$ be an arbitrary integer, and assume $n$ is even.

- Since the product of any number with an even number is even,

- $7n$ must be even.

2.

Q: Arrange some of the statements below to form a correct proof of the following
statement: "For any integer $n$, if $7n$ is even, then $n$ is even."

- Let $n$ be an arbitrary integer, and assume $n$ is even.

- Since the $7$ is odd and the product of an odd number with an even number is
  even,

- $7n$ must be even.

- Let $n$ be an arbitrary integer, and assume $7n$ is even.

- Since an even number divided by $7$ must be even,

- $n$ must be even.

- Let $n$ be an arbitrary integer, and assume $n$ is odd.

- Since $7$ is odd and the product of an odd number and an odd number is odd,

- $7n$ must be odd.

A:

The contrapositive proof starts with Assume the conclusion is false, and
conclude therefore that the assumption is false.

$$ \neg Q \to \neg P $$

So our proof by contrapositive would look like:

- Let $n$ be an arbitrary integer, and assume $n$ is odd.

- Since $7$ is odd and the product of an odd number and an odd number is odd,

- $7n$ must be odd.

3.

Q: Consider the statement, "For any numbers $a$ and $b$, if $a + b$ is odd, then
either $a$ or $b$ is odd."

Give a valid proof of the statement using a _proof by contrapositive_. Arrange
some statements below to complete the proof.

- Let $a$ and $b$ be integers, and assume that $a + b$ is odd.

- Let $a$ and $b$ be integers, and assume that if $a + b$ is odd, then either
  $a$ or $b$ is odd.

- Let $a$ and $b$ be integers, and assume both are even.

- The sum of two even integers must also be even.

- Therefore $a + b$ is even.

- Let $a$ and $b$ be integers and assume that $a + b$ is odd but $a$ and $b$ are
  both even.

- The sum of two odd integers must be even.

- But then $a + b$ is both even and odd, a contradiction.

A:

A proof by contrapositive starts with assuming that the original statement's
consequent is false, and concludes that the original statement's antecedent is
false.

$$ \neg Q \to \neg P $$

$\neg Q$ would be something like "For any numbers $a$ and $b$, it is false that
either are odd, so both $a$ and $b$ are even."

$\neg P$ would be something like "$a + b$ is even."

So the order of our proof would be:

- Let $a$ and $b$ be integers, and assume both are even.

- The sum of two even integers must also be even.

- Therefore $a + b$ is even.

4.

Q: Consider the same statement, "For any numbers $a$ and $b$, if $a + b$ is odd,
then either $a$ or $b$ is odd."

Give a valid proof of the statement, this time using a _proof by contradiction_
using some of the statements below.

- Let $a$ and $b$ be integers, and assume that $a + b$ is odd.

- Let $a$ and $b$ be integers, and assume that if $a + b$ is odd, then either
  $a$ or $b$ is odd.

- Let $a$ and $b$ be integers, and assume both are even.

- The sum of two even integers must also be even.

- Therefore $a + b$ is even.

- Let $a$ and $b$ be integers and assume that $a + b$ is odd but $a$ and $b$ are
  both even.

- The sum of two odd integers must be even.

- But then $a + b$ is both even and odd, a contradiction.

A:

A proof by contradiction starts with assuming the negation of our original
statement, and then concluding with a statement that is a contradiction.

$$ \neg(P \to Q) $$

It might be helpful to use negation is disjunction and De Morgan's laws here:

$$ \neg(\neg P \vee Q) $$

$$ P \wedge \neg Q $$

Which reads something like "For any numbers $a$ and $b$, $a + b$ is odd and
$a + b$ is even." That's a contradiction. Let's see how we can order our given
choices to create a proof statement.

Proof by contradiction:

- Let $a$ and $b$ be integers and assume that $a + b$ is odd but $a$ and $b$ are
  both even.

- The sum of two even integers must also be even.

- But then $a + b$ is both even and odd, a contradiction.

5.

Q: Below are three statements that together with a possible first line of a
proof of that statement. In each case, say whether the first line is the start
of a direct proof, a proof by contrapositive, or a proof by contradiction.

(a)

**_Statement:_** For every integer $n$, the number $7n - 1$ is divisible by $6$.

**_First line:_** Suppose there were some integer $n$ for which $7n - 1$ was not
divisible by $6$.

(b)

**_Statement:_** For any integer $n$, if $n$ is prime, then $n$ is solitary.

**_First line:_** Let $n$ be an integer, and assume $n$ is not solitary.

\(c\)

**_Statement:_** If a shape is a pentagon, then its interior angles add up to
480 degrees.

**_First line:_** Consider an arbitrary shape, and assume it is a pentagon.

A:

(a)

**_Statement:_** For every integer $n$, the number $7n - 1$ is divisible by $6$.

**_First line:_** Suppose there were some integer $n$ for which $7n - 1$ was not
divisible by $6$.

We can approach this by first defining what the antecedent and the consequent
is:

$P(n)$ is "Suppose there were some integer $n$"

$Q(n)$ is "There exists a number $7n - 1$ that is divisible by $6$."

The first line states a negation of the original statement, this is the start to
a Proof by Contradiction.

(b)

**_Statement:_** For any integer $n$, if $n$ is prime, then $n$ is solitary.

**_First line:_** Let $n$ be an integer, and assume $n$ is not solitary.

$P(n)$ is "$n$ is prime."

$Q(n)$ is "$n$ is solitary."

The first line starts with a negation of the original consequent, this is the
start to a Proof by Contrapositive.

\(c\)

**_Statement:_** If a shape is a pentagon, then its interior angles add up to
480 degrees.

**_First line:_** Consider an arbitrary shape, and assume it is a pentagon.

$P$ is "the shape is a pentagon."

$Q$ is "its interior angles add up to 480 degrees."

The first line assumes the assumption of the original statement, this is a
Direct Proof.

6.

Q: What would the first line be for a proof in each style, of the following
statement:

"If a function $f : A \to B$ is a bijection, then |A| = |B|."

$\text{Assume } f : A \to B \text{ is a bijection} \quad \text{ Direct proof}$

$\text{Assume } f: A \to B \text{ is a bijection and } |A| \neq |B| \quad \text{ Proof by contrapositive}$

$\text{Assume} |A| \neq |B| \quad \text{ Proof by contradiction}$

A:

Yes, this first one needs no adjustment, this is the first line of a Direct
proof:

$\text{Assume } f : A \to B \text{ is a bijection} \quad \text{ Direct proof}$

The next one negates the entire original statement, that is a first line of a
Proof by Contradiction:

$\text{Assume } f: A \to B \text{ is a bijection and } |A| \neq |B| \quad \text{ Proof by contradiction}$

The next one negates the original consequent, and so is the first line of a
Proof by Contrapositive:

$\text{Assume} |A| \neq |B| \quad \text{ Proof by contrapositive}$
