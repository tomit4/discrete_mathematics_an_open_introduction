# Preview Activity

In this preview activity, we will explore some basic properties of sets and
functions. Later in this section, we will write proofs about these ideas.

1.

Remember that a set is just a collection of elements. Here are two definitions
about sets:

a. A set $A$ is a subset of $B$, written $A \subseteq B$, provided every element
in $A$ is also an element of $B$.

b. Given sets $A$ and $B$, the union of $A$ and $B$, written $A \cup B$, is the
set containing every element that is in $A$ and $B$ or both.

(a)

Q: Let$B = \{1, 3, 5, 7, 9\}$. Give an example of a set $A$ containing 3
elements that is a subset of $B$.

What is $A \cup B$ for a set $A$ you gave as an example?

A:

$$ A = \{1, 3, 5\} $$

$$ A \cup B = \{1, 3, 5, 7, 9\} $$

(b)

Q: Give an example of two distinct sets $A$ and $B$ such that $A \cup B = B$.

For the example you gave, is $A \subseteq B$?

A:

$$ A = \{1, 2\}, \quad B = \{1, 2, 3\} $$

Yes, for this example, $A \subseteq B$.

\(c\)

Q: Find examples, if they exist, of sets $A$ and $B$ such that
$A \cup B \neq B$.

For the example you gave, is $A \subseteq B$?

A:

$$ A = \{1, 2, 3\} \quad B = \{1, 2\} $$

$$ A \cup B = \{1, 2, 3\} $$

In this case $A$ is not a subset of $B$.

2.

Which of the following are always true?

A.

Q: For any sets $A$ and $B$, $A \cup B \subseteq B$.

A: No, we just demonstrated that this was not true in 1a by showing example sets
this is not the case.

B.

Q: For any sets $A$ and $B$, $B \subseteq A \cup B$.

A: Yes this is always true. Since $A \cup B$ will always contain elements from
both $A$ and $B$, this means that every element of $B$ is automatically in
$A \cup B$.

C.

Q: For any sets $A$ and $B$, if $A \subseteq B$, then $A \cup B \subseteq B$.

A: Yes this is always true. $A \subseteq B$ means that set $B$ contains all
elements of $A$, and so therefore the union of $A \cup $B$ will always be a
subset of $B$.

D.

Q: For any sets $A$ and $B$, if $A \cup B = B$, then $A \subseteq B$.

A: Yes, this is always true. If $A \cup B = B$, this means that any element in
$A$ must also be in $B$, but $A$ must also not contain any elements not in $B$.
This makes $A$ a subset of $B$.

3.

For any function $f:\mathbb{N} \to \mathbb{N}$ and any set
$A \subseteq \mathbb{N}$, we can define the image of $A$ under $f$ to be the set
of all outputs of $f$ when the input is an element of $A$. We write this as
$f(A) = \{f(x) : x \in A\}$.

For the following tasks, let's explore the function
$f : \mathbb{N} \to \mathbb{N}$ defined by $f(x) = x^2 - 3x + 8$.

(a)

Q: Let $A = \{1, 2, 3\}$ and $B = \{2, 4, 6\}$. Find $f(A)$ ad $f(B)$. Then find
$f(A) \cup f(B)$.

A:

$$ f(A) = \{6, 8 \} $$

$$ f(B) = \{12, 26\}  $$

$$ f(A) \cup f(B) = \{6, 8, 12, 26\} $$

(b) Now find $A \cup B$ and $f(A \cup B)$.

$$ A \cup B = \{1, 2, 3, 4, 6\} $$

$$ f(A \cup B) = \{6, 8, 12, 26\} $$

\(c\)

Q: Give an example, if one exists, of two distinct sets $A$ and $B$ such that
$A \subseteq B$ and $f(A) \subseteq f(B)$.

A:

$$ A = \{1, 2\} \quad B = \{1, 2, 3\} $$

$$ A \subseteq B $$

$$ f(A) = \{6\} $$

$$ f(B) = \{6, 8\} $$

$$ f(A) \subseteq f(B) $$

Q: Give an example, if one exists, of two distinct sets $A$ and $B$ such that
$A \subseteq B$ but $f(A) \nsubseteq f(B)$.

A:

The requested example cannot exist.
