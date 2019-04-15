# in-place selection sort

Rearrange
an unordered `ArrayList<Integer>`
and use it as the data in an `OrderedList_inArraySlots`.

The re-use is probably contrary to Java's conventions
for its built-in classes. But as a pedagogical tool,
it has the advantage of allowing
the User program to check that the sort
is done in-place.

## count the cost

0. If the number of the elements in the input triples,
the time required to run the reigning champ algorithm
will grow by about 9 times. If the sum of the arithmetic
sequence is n(A1 +An) / 2, tripling element count triples
both n and An (roughly), resulting in about 9 times.

1. If the number of the elements in the input triples,
the number of times that the reigning champ algorithm
will be invoked will grow by 3 times. The algorithm is
invoked for every element, so tripling element count
triples the number of times the algorithm is invoked.

2. If the number of the elements in the input triples,
the time required for the selection sort will grow by
9 times. We effectively have a nested 'for' loop, each
for loop must visit each element once, so tripling the
element count will increase time for selection sort by
3 * 3 = 9 times.
