1.

Q:

The most popular mathematician in the world is throwing a party for all of his
friednds. To kick things off, they decide that everyone should shake hands.
Assuming all 10 people at the party each shake hands with every other person
(but not themselves, obviously) exactly once, how many handshakes take place?

1A:

If we pair off the people into sets, then we get something like this:

{1, 2}, {1, 3}, {1, 4}, {1, 5}, {1, 6}, {1, 7}, {1, 8}, {1, 9}, {1, 10}

{2, 3}, {2, 4}, {2, 5}, {2, 6}, {2, 7}, {2, 8}, {2, 9}, {2, 10}

{3, 4}, {3, 5}, {3, 6}, {3, 7}, {3, 8}, {3, 9}, {3, 10}

{4, 5}, {4, 6}, {4, 7}, {4, 8}, {4, 9}, {4, 10}

{5, 6}, {5, 7}, {5, 8}, {5, 9}, {5, 10}

{6, 7}, {6, 8}, {6, 9}, {6, 10}

{7, 8}, {7, 9}, {7, 10}

{8, 9}, {8, 10}

{9, 10}

As you can see this just becomes 10+9+8+7+6+5+4+3+2+1=55 handshakes. This likely
is alluding to basic summation mathematical induction.

2.

Q: At the warm-up event for Oscar's All-Star Hot Dog Eating Contest, Al ate one
hot dog. Bob then showed him up by eating three hot dogs. Not to be outdone,
Carl ate five. This continued with each contestant eating two more hot dogs than
the previous contestant. How many hot dogs did Zeno (the 26th and final
contestant) eat? How many hot dogs were eaten in total?

A:

This is another summation mathematical induction function, just slightly
different:

(1) +

(1 + 2) +

(3 + 2) +

(5 + 2) +

(7 + 2) +

(9 + 2) +

(11 + 2) +

(13 + 2) +

(15 + 2) +

(17 + 2) +

(19 + 2) +

(21 + 2) +

(23 + 2) +

(25 + 2) +

(27 + 2) +

(29 + 2) +

(31 + 2) +

(33 + 2) +

(35 + 2) +

(37 + 2) +

(39 + 2) +

(41 + 2) +

(43 + 2) +

(45 + 2) +

(47 + 2) +

(49 + 2) +

(51 + 2) +

(53 + 2) = 55

(1) + (1 + 2) + (3 + 2) + (5 + 2) + (7 + 2) + (9 + 2) + (11 + 2) + (13 + 2) +
(15 + 2) + (17 + 2) + (19 + 2) + (21 + 2) + (23 + 2) + (25 + 2) + (27 + 2) +
(29 + 2) + (31 + 2) + (33 + 2) + (35 + 2) + (37 + 2) + (39 + 2) + (41 + 2) +
(43 + 2) + (45 + 2) + (47 + 2) + (49 + 2) + (51 + 2) + (53 + 2) = 784

55 is how many Zeno ate, and the total hot dogs that were eaten is : 784

3.

Q: After excavating for weeks, you finally arrive at the burial chamber. The
room is empty except for two large chests. On each is carved a message
(strangely English):

- Exactly one of these chests contains a treasure, while the other is filled
  with deadly immortal scorpions.

- For either chest, if the chest's message is true, then the chest contains
  treasure.

The problem is, you don't know whether the messages are true or false. What do
you do?

A: Honestly, I'd probably walk away, but since that's likely not the answer,
we'd likely have to consider that these are relating to a form of truth tables.

The first chest's message claims that one chest contains scorpions, the other
treasure

So if we say T="contains treasure", and f="contains scorpions", then we can say
that Chest_1 and Chest_2:

Chest_1 = T Chest_2 = F

The other chest's message claims that if it's own message or the other chest's
message is true, then the chest contains treasure.

This is a contradiction, because if the second chest's message is true, then
that chest is the one that contains treasure, and the other chest is the one
that contains scorpions.

If the second chest's message is false, then the chest doesn't contain treasure,
but then you don't know if the second chest contains treasure or scorpions,
because the chest containing treasure is no longer contingent on whether the
chest's message is true or not.

This is probably best expressed again, in some form, of truth notation.

4.

Q: Back in the days of yore, five small towns decided they wanted to build roads
directly connecting each pair of towns. While the towns had plenty of money to
build roads as long and as winding as they wished, it was very important that
the roads not intersect with each other (as stop signs had not yet been
invented). Also, tunnels and bridges were not allowed, for moral reasons. It is
possible for each of these towns to build a road to each of the four other towns
without creating any intersections?

A: This seems possible, as you could just create two roads from each town to at
least two other towns (a pair as the question alludes to). But something tells
me this is a trick question.
