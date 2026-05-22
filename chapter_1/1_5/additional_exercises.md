# 1.5.8 Additional Exercises

1.

Q: Prove that for any two sets $A$ and $B$, $A \subseteq B$ if and only if
$A \cup B = B$.

A:

First, let's prove that for any two sets $A$ and $B$, $A \subseteq B$ if
$A \cup B = B$.

$$ A \cup B = B \to A \subseteq B $$

- Suppose that $A \cup B = B$.

- Let $x$ be in $A$, $x \in A$.

- Then $x \in A \cup B$.

- Since $A \cup B = B$, then $x \in B$.

- Therefore $A \subseteq B$

Second, let's prove that for any two sets $A$ and $B$, $A \cup B = B$, if
$A \subseteq B$.

$$ A \subseteq B \to A \cup B = B $$

- Suppose $A \subseteq B$

- Let $x \in A \cup B$

- Then $x \in A$ or $x \in B$ by definition of a union.

- If $x \in B$, done.

- If $x \in A$, then since $A \subseteq B$, we get $x \in B$.

- So, in all cases $x \in B$.

- Therefore $A \cup B \subseteq B$.

2.

Q: The **intersection** of sets $A$ and $B$, denoted $A \cap B$, is the set of
all elements that are in both $A$ and $B$.

Prove that for any two sets $A$ and $B$, $A \subseteq B$ if and only if
$A \cap B = A$.

A:

First, let's prove:

$$ A \subseteq B \to A \cap B = A $$

- Suppose that $A \subseteq B$

- Let $x$ be some element such that $x \in A \cap B$

- Since $A \subseteq B$, and $x \in A \cap B$, then $x \in A$ by definition of
  an intersection

- Therefore $A \cap B \subseteq A$.

Secondly, let's prove:

$$ A \cap B = A \to A \subseteq B $$

- Suppose that $A \cap B = A$.

- Let $x$ be some element such that $x \in A$.

- Since $A \cap B = A$ and $x \in A$, then $x \in A \cap B$.

- $x \in A \cap B$ means $x$ \in A$ and $x \in B$ by definition of an
  intersection

- Since every element of $A$ is an element of $B$, therefore $A \subseteq B$

3.

Q: Prove that for any sets $A$, $B$, and $C$, if $A \cup B \subseteq C$, then
$A \subseteq C$ and $B \subseteq C$.

A:

First, let us prove:

$$ A \cup B \subseteq C \to A \subseteq C $$

- Suppose $A \cup B \subseteq C$

- Let $x$ be an element such that $x \in A$

- Since $x \in A$, we know that $x \in A \cup B$, by definition of a union.

- Since we know that $A \cup B \subseteq C$, it follows that $x \in C$.

- Therefore $A \subseteq C$

Second, let's prove that $B \subseteq C$:

$$ A \cup B \subseteq C \to B \subseteq C $$

- Suppose that $A \cup B \subseteq C$

- Let $x$ be an element such that $x \in B$

- Since $x \in B$, it follows that $x \in A \cup B$, by definition of a union

- Since we know that $A \cup B \subseteq C$, it follows that $x \in C$.

- Therefore $B \subseteq C$

4.

Q: Prove that for any sets $A$, $B$, and $C$, if $A \subseteq C$ and
$B \subseteq C$, then $A \cup B \subseteq C$.

A:

Let's prove:

$$ (A \subseteq C) \wedge (B \subseteq C) \to A \cup B \subseteq C $$

- Suppose that $A \subseteq C$

- Suppose that $B \subseteq C$

- Let $x$ be an element such that $x \in A \cup B$

- $x \in A \cup B$ means that $x \in A$ or $x \in B$ by definition of a union

- If $x \in A$, and $A \subseteq C$, then $x \in C$

- If $x \in B$, and $B \subseteq C$, then $x \in C$

- In both cases $x \in C$

- Therefore $A \cup B \subseteq C$

5.

Q: The **difference** of sets $A$ and $B$, written $A \setminus B$, is the set
of all elements that are in $A$ but not in $B$.

The **empty set**, written $\emptyset$, is the set that contains no elements.

Prove that if $A \setminus B = A$ then $A \cap B = \emptyset$.

A:

Let's prove:

$$ A \setminus B = A \to A \cap B = \emptyset $$

- Suppose $A \setminus B = A$

- Let $x$ be an element such that $x \in A \cap B$

- Since $x \in A \cap B$, this means that $x \in A$ and $x \in B$ by definition
  of an intersection

- Since $A \setminus B = A$ and $x \in A$, it follows that $x \in A \setminus B$

- But if $x \in A \setminus B$, then it follows that $x \notin B$

- This is a contradiction since we established earlier that $x \in B$ by
  definition of an intersection, but now we also established that $x \notin B$.

- Therefore $A \cap B = \emptyset$

A small note is worthwhile here. This is not a proof by contradiction in the
traditional sense. The contradiction does not start at the premise/argument
level, it only occurs at a single step of the proof.

6.

Q: Prove that if $A \setminus B = B \setminus A$ then $A = B$.

A:

Let's prove:

$$ (A \setminus B = B \setminus A) \to A = B $$

- Suppose that $A \setminus B = B \setminus A$

- Let $x$ be an element such that $x \in A \setminus B$

- Since $x \in A \setminus B$, this means that $x \in A$ and $x \notin B$ by
  definition of a difference

- Since $x \in A \setminus B$ and $A \setminus B = B \setminus A$, it follows
  that $x \in B \setminus A$

- Since $x \in B \setminus A$, this means that $x \in B$ and $x \notin A$ by
  definition of a difference

- This is a contradiction since we've established that $x \in A$, $x \notin A$
  (and also $x \in B$ and $x \notin B$).

- Therefore since $x$ cannot exist, we can conclude that
  $A \setminus B = \emptyset$.

- And since $A \setminus B = \emptyset$ and $A \setminus B = B \setminus A$, we
  can further conclude that $B \setminus A = \emptyset$.

- Since $A \setminus B = \emptyset$, we can conclude that $A \subseteq B$

- And also since $B \setminus A = \emptyset$, we can further conclude that
  $B \subseteq A$

- Therefore $A = B$

7.

Q: Let $f:X \to Y$ be a function, and let $A$ and $B$ be subsets of $X$.

(a) Prove that $f(A \cap B) \subseteq f(A) \cap f(B)$.

(b) Find an example of a function and two sets $A$ and $B$ such that
$f(A \cap B) \neq f(A) \cap f(B)$.

A:

(a) Prove that $f(A \cap B) \subseteq f(A) \cap f(B)$.

- Let there be some output $y$ such that $y \in f(A \cap B)$.

- Since $y \in f(A \cap B)$, there exists $x \in A \cap B$ such that $f(x) = y$
  by the definition of an image.

- Since $x \in A \cap B$, this means that $x \in A$ and $x \in B$ by definition
  of an intersection.

- It then follows that $f(x) \in f(A)$ and $f(x) \in f(B)$.

- Since $f(x) = y$, it further follows that $y \in f(A)$ and $y \in f(B)$, which
  is expressed as $y \in f(A) \cap f(B)$.

- Therefore $f(A \cap B) \subseteq f(A) \cap f(B)$

(b) Find an example of a function and two sets $A$ and $B$ such that
$f(A \cap B) \neq f(A) \cap f(B)$.

A: This can happen depending on exactly what the function $f$ is in this case
and what $A$ and $B$ are defined as.

Let's say that $f$ in this case is:

$$ f(x) = 0, x \in \mathbb{R} $$

Then let's say our sets are:

$$ A = \{0\} $$

$$ B = \{1\} $$

Then for $f(A \cap B)$, we'll first need $A \cap B$:

$$ A \cap B = \emptyset $$

So:

$$ f(A \cap B) = f(\emptyset) = \emptyset $$

A small note here: when applying a function to a set via image notation, if the
set is empty, then there are no elements to map under the function, so the image
is the empty set.

Then consider $f(A) \cap f(B)$:

$$ f(\{0\}) = \{0\} $$

$$ f(\{1\}) = \{0\} $$

So:

$$ f(A) \cap f(B) = \{0\} $$

And then when we make our comparison:

$$ f(A \cap B) = \emptyset \neq \{0\} = f(A) \cap f(B) $$

So this is an example where:

$$ f(A \cap B) \neq f(A) \cap f(B) $$

8.

Q: Let $f: X \to Y$ be a function, and let $A$ and $B$ be subsets of $X$.

(a) Prove that $f(A \cup B) \subseteq f(A) \cup f(B)$.

(b) Prove that $f(A) \cup (B) \subseteq f(A \cup B)$

\(c\) What can you conclude from the two proofs above?

A:

(a) Prove that $f(A \cup B) \subseteq f(A) \cup f(B)$.

- Let there be some output $y$ such that $y \in f(A \cup B)$.

- Since $y \in f(A \cup B)$, there exists $x \in A \cup B$ such that $f(x) = y$
  by the definition of an image.

- Since $x \in A \cup B$, this means that $x \in A$ or $x \in B$ by definition
  of an union.

- It then follows that $f(x) \in f(A)$ or $f(x) \in f(B)$.

- Since $f(x) = y$, it further follows that $y \in f(A)$ or $y \in f(B)$, which
  is expressed as $y \in f(A) \cup f(B)$.

- Therefore $f(A \cup B) \subseteq f(A) \cup f(B)$

(b) Prove that $f(A) \cup (B) \subseteq f(A \cup B)$

- Let there be some output $y$ such that $y \in f(A) \cup f(B)$.

- Since $y \in f(A) \cup f(B)$, this means that $y \in f(A)$ or $y \in f(B)$ by
  definition of a union.

- Since $y \in f(A) \cup f(B)$, there exists $x \in A$ or there exists $x \in B$
  such that $f(x) = y$ by the definition of an image.

- If $x \in A$, $x \in A \cup B$.

- If $x \in B$, $x \in A \cup B$.

- In both cases $x \in A \cup B$, so $y \in f(A \cup B)$

- Since $f(x) = y$, it further follows that $y \in f(A \cup B)$.

- Therefore $f(A) \cup f(B) \subseteq f(A \cup B)$

\(c\) What can you conclude from the two proofs above?

Since in part (a), we found that $f(A \cup B) \subseteq f(A) \cup f(B)$ and in
part (b) we found that $f(A) \cup f(B) \subseteq f(A \cup B)$, we can conclude
that:

$$ f(A \cup B) = f(A) \cup f(B) $$

9.

Q: Given a function $f: X \to Y$ and a set $B \subseteq Y$, we define the
**inverse image** of $B$ under $f$ as the set
$f^{-1}(B) = \{x \in X: f(x) \in B\}$. That is, it is all the elements in the
domain that are mapped to elements in $B$.

(A) For $f: \mathbb{N} \to \mathbb{N}$ defined by $f(n) = n^2$, what are each of
the following sets?

(a) $f^{-1}(\{1, 4, 9\})$

(b) $f^{-1}(\{2, 3, 5, 7\})$

\(c\) $f^{-1}(\{1, 2, \dots, 10\})$

(B) Prove that for any set $C \subseteq X, C \subseteq f^{-1}(f(C))$.

\(C\) Give an example of a function $f$ and a set $C$ such that
$C \neq f^{-1}*(f(C))$.

(D) Prove that for any set $D \subseteq Y, f(f^{-1}(D)) \subseteq D$.

(E) Give an example of a function $f$ and a set $D$ such that
$f(f^{-1}(D)) \neq D$.

A:

(A) For $f: \mathbb{N} \to \mathbb{N}$ defined by $f(n) = n^2$, what are each of
the following sets?

(a) $f^{-1}(\{1, 4, 9\})$

$$ f^{-1}(\{1, 4, 9\}) = \{1, 2, 3\} $$

(b) $f^{-1}(\{2, 3, 5, 7\})$

$$ f^{-1}(\{2, 3, 5, 7\}) = \emptyset $$

There are no natural numbers, $n$ such that $n^2 \in \{2, 3, 5, 7\}$ since none
of these numbers are perfect squares.

\(c\) $f^{-1}(\{1, 2, \dots, 10\})$

$$ f^{-1}(\{1, 2, \dots, 10\}) = \{1, 2, 3\} $$

(B) Prove that for any set $C \subseteq X, C \subseteq f^{-1}(f(C))$.

- Let $x$ be some element $x \in C$.

- If we then apply the function $f$ to $x$ as $f(x)$, since $C \subseteq X$, it
  follows that $f(x) \in f(C)$ by the definition of the image of a set.

- Since $f(x) \in f(C)$, it then follows that $x \in f^{-1}(f(C))$ by definition
  of an inverse image of a set.

- Therefore $C \subseteq f^{-1}(f(C))$.

\(C\) Give an example of a function $f$ and a set $C$ such that
$C \neq f^{-1}*(f(C))$.

- Let $X$ be the set $\{1, 2\}$, and let $C$ bu a subset of $X$, $C \subseteq X$
  such that $C = \{1\}$.

- Let $f$ be a function defined as:

$$ f: X \to Y \quad f(x) = 0 \forall x \in X $$

- Therefore $f(C) = \{0\}$

- By the definition of an inverse image of a set
  $f^{-1}(f(C)) = \{x \in X: f(x)\in f(C)\}$, so therefore
  $f^{-1}(f(C)) = \{x \in X: f(x) = 0\}$

- Since $X = \{1, 2\}$, then $f(1) = 0$ and $f(2) = 0$, so
  $f^{-1}(C) = \{1, 2\}$.

- Therefore $C = \{1\}$ and $f^{-1}(f(C)) = \{1, 2\}$, which means that
  $C \neq f^{-1}(f(C))$.

(D) Prove that for any set $D \subseteq Y, f(f^{-1}(D)) \subseteq D$.

- By definition of an inverse image:

$$ f^{-1}(D) = \{x \in X: f(x) \in D\} $$

- By applying $f$ to the inverse, we get:

$$ f(f^{-1}(D)) = \{f(x): x \in X, f(x) \in D\} $$

- Since $x \in f^{-1}(D)$, we have $f(x) \in D$, so every element of
  $f(f^{-1}(D))$ lies in $D$.

- Therefore, $f(f^{-1}(D)) \subseteq D$.

(E) Give an example of a function $f$ and a set $D$ such that
$f(f^{-1}(D)) \neq D$.

- Let the following be:

$$ X = \{1, 2} $$

$$ Y = \{0, 1\} $$

$$ f(1) = 0, f(2) = 0 $$

$$ D = \{0, 1\} $$

- The inverse image is:

$$ f^{-1}(D) = \{1, 2\} $$

- Apply $f$ to the inverse:

$$ f(f^{-1}(D)) = f(\{1, 2\}) = \{0\} $$

- Comparing:

$$ f(f^{-1}(D)) = \{0\} \neq \{0, 1\} = D $$

10.

Q: Let $f: X \to Y$ be a function, and let $A$ and $B$ be subsets of $Y$. Prove
that $f^{-1}(A \cap B) = f^{-1}(A) \cap f^{-1}(B)$.

A:

- Let $x \in f^{-1}(A \cap B)$.

- By definition of an inverse image, this means that $f(x) \in A \cap B$

- This means that $f(x) \in A \wedge f(x) \in B$ by definition of an
  intersection.

- It follows then that $x \in f^{-1}(A) \cap f^{-1}(B)$

- Therefore $f^{-1}(A \cap B) \subseteq f^{-1}(A) \cap f^{-1}(B)$

To prove equality, we must also show the reverse inclusion.

- Let $x \in f^{-1}(A) \cap f^{-1}(B)$.

- This means that $x \in f^{-1}(A) \wedge x \in f^{-1}(B)$ by definition of an
  intersection.

- It follows then that $f(x) \in A \wedge f(x) \in B$ by definition of an image
  of a set.

- Then $f(x) \in A \cap B$ by definition of an intersection.

- So $x \in f^{-1}(A \cap B)$ by definition of an inverse image of a set.

- Therefore $f^{-1}(A) \cap f^{-1}(B) \subseteq f^{-1}(A \cap B)$

Since both inclusions hold, this proves that:

$$ f^{-1}(A \cap B) = f^{-1}(A) \cap f^{-1}(B) $$

11.

Q: Let $f: X \to Y$ be a function, and let $A$ and $B$ be subsets of $Y$. Prove
that $f^{-1}(A \cup B) = f^{-1}(A) \cup f^{-1}(B)$.

A:

- Let $x \in f^{-1}(A \cup B)$

- Then $f(x) \in A \cup B$ by definition of an inverse image.

- This means that $f(x) \in A \vee f(x) \in B$ by definition of a union.

- It follows then that $x \in f^{-1}(A) \vee x \in f^{-1}(B)$ by definition of
  an inverse image.

- So $x \in f^{-1}(A) \cup f^{-1}(B)$ by definition of a union.

- Therefore $f^{-1}(A \cup B) \subseteq f^{-1}(A) \cup f^{-1}(B)$

Now reverse the inclusion.

- Let $x \in f^{-1}(A) \cup f^{-1}(B)$

- Then $x \in f^{-1}(A) \vee x \in f^{-1}(B)$ by definition of a union.

- So $f(x) \in A \vee f(x) \in B$ by definition of an inverse image.

- It then follows that $f(x) \in A \cup B$ by definition of a union.

- So $x \in f^{-1}(A \cup B)$ by definition of an inverse image.

- Therefore $f^{-1}(A) \cup f^{-1}(B) \subseteq f^{-1}(A \cup B)$

Since both inclusions hold, we have proved that:

$$ f^{-1}(A \cup B) = f^{-1}(A) \cup f^{-1}(B) $$

12.

Q: For each relation below, determine whether it is transitive. If it is, prove
it. If it is not, give a counterexample.

(a) The relation "$|$" (divides) on $\mathbb{Z}$ defined by $a|b$ provided $b$
is a multiple of $a$.

$a|b$ is transitive on $\mathbb{Z}$ provided $b$ is a multiple of $a$.

Let $k$ be some multiple of $a$, this means that:

$$ b = a \cdot k $$

Let $c$ then be a multiple of $b$, $c|b$. Then let $m$ be some multiple of $c$.
This would then mean that:

$$ c = b \cdot m $$

$$ c = (a \cdot k) \cdot m = a(km) $$

And this means then that $c$ is a multiple of $b$ and also $a$ and that $a|b|c$.
Therefore the property is transitive since this then means that $a|c$.

(b) The relation "$\leq$" (less than or equal to) on $\mathbb{R}$.

The relation $\leq$ is transitive.

If we have two numbers, $b$, and $c$ such that $b \leq c$, and then we also have
a number $a$, such that $a \leq b$ , then it is true that $a \leq c$, which
demonstrates the transitive property.

\(c\) The relation "$\perp$" (is perpendicular to) on the set of lines in the
plane.

The relation $\perp$ is not transitive. Consider one horizontal plane $a$ and a
vertical plane $b$ such that $a \perp b$. Then say you have another horizontal
plane $c$ such that $b \perp c$. But this does NOT mean that $a \perp c$ since
this means that $a$ and $c$ are actually horizontal to each other, i.e.
$\overline{ac}$.

(d) The relation "$\sim$" (is similar to) on the set of triangles in the plane
(two triangles are similar if they have the same angles, bu are not necessarily
the same size).

The relation $\sim$ is transitive. Consider two triangles $A$ and $B$ such that
$A \sim B$. This means that both $A$ and $B$ have the same angles (but not
necessarily the same leg dimensions). If we then have a third triangle, $C$,
such that $B \sim C$, then this means that both $B$ and $C$ have the same angles
(but again, not necessarily the same leg dimensions). Since $A$ and $B$ have the
same angles (are $\sim$), and $B$ and $C$ have the same angles (are $\sim$),
then we can conclude that $A \sim C$ and we have shown that the relation $\sim$
is transitive.
