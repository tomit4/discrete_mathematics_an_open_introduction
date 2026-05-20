# Investigate!

Q: Suppose there are 15 people at a party. Most people know each other already,
but there are still some people who decide to shake hands. Is it possible for
everyone at the party to shake hands with exactly three other people?

A:

Let $n$ be the amount of people at the party. Since every person must shake
hands with exactly 3 people, then we can represent the amount of handshakes that
takes place at the party to be $3n$.

To determine if we have enough people at the party where everyone gets to shake
the hand of exactly three other people, we can utilize what is known as the
[Pigeonhole Principle](https://en.wikipedia.org/wiki/Pigeonhole_principle) where
instead of pigeons we consider the amount of handshakes $3n$ and then evaluate
the remainder of how many containers, or "handshake contributions" every
handshake creates, in this case $2$.

To understand this, consider that every time a single person shakes another
person's hands, it counts as 2 handshakes:

Alice shakes Bob's hand, but Bob also shakes Alice's hands. For the context of
this problem, 2 handshakes occur every time two individuals shake hands.

If we tally up the total amount of handshakes that must take place at this
party:

$$ 3n =  3 * 15 = 45 \text{ handshake contributions} $$

And we look at the remainder of how many handshakes are contributed:

$$ 45 \not\equiv 0 \mod 2$$

We can see that we'll always need an even amount of people at this party for
everyone to be able to shake the hands of exactly 3 people.
