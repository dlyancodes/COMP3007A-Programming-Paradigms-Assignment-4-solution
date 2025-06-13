# COMP3007A-Programming-Paradigms-Assignment-4-solution

Download Here: [COMP3007A “Programming Paradigms” Assignment 4 solution](https://jarviscodinghub.com/assignment/comp3007a-programming-paradigms-specification-for-assignment-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Question 1: “Structural Induction”
For this question, you must consider the following definition and functions for the NTree
data type (below) and prove (using structural induction) that for every binary tree Z:
count Z  2(height Z) – 1
Remember that, if you are trying to prove that b  d, and you know that a  b  c, you can
replace b with c (to get c  d) but you cannot replace b with a (to get a  d). To receive full
marks for this question you must show every step in your proof and you must use the source
code line labels (shown below, in red) whenever you use equational reasoning.
data NTree = NilT | Node Int NTree NTree
[ctb] count NilT = 0
[ctr] count (Node n x y) = (count x) + (count y) + 1
[htb] height NilT = 0
[htr] height (Node n x y) = (max (height x) (height y)) + 1
max a b
[mc1] | a >= b = a
[mc2] | otherwise = b
COMP3007A (Fall 2018)  “Programming Paradigms”
Specification for Assignment 4 of 4
Question 2: “Count Elements from Range”
A function to count the number of elements in a list of integers that are within some range
(inclusively) is straightforward in either Haskell or Prolog. In Haskell, it would have three
parameters (the list of integers and the lower and upper bound of the) and would return a
single value (the number of elements within that range). In Prolog, it would be a predicate of
arity four that succeeds when the fourth element is the number of elements in the first list
argument that are in the range specified by the second and third arguments (and you could
leave the fourth element uninstantiated to have Prolog count it for you).
HASKELL > countInRange [2,4,6,8,10,12,14,16,18] 3 11
4
PROLOG ?- countInRange([2,4,6,8,10,12,14,16,18], 3, 11, X).
X = 4 ;
false.
For this question, you will write this function twice – once using Haskell and once using Prolog.
Both solutions must be recursive, the Haskell solution must be tail-call optimized, and neither
solution may use higher order functions.
Question 3: “You SHALL Pass”
For this question, you must write a Prolog program that will solve the following logic puzzle
by modeling it as a finite state machine. Your solution to this question must answer True or
False for the first question (i.e., Is it possible…?) and it must provide an unambiguous
description of the action plan for the second question (i.e., How?).
While traveling through Moria, Gandalf, Aragorn, Gilmi, and Legolas approach a great chasm.
There is a bridge going across but it can only hold two people at a time. Because of poor
planning, they only have a single torch between the four of them, and since the mines are
particularly dark, the torch must be carried whenever someone tries to cross the bridge.
Legolas is the fastest and can cross the bridge in only one minute, and Aragorn is in pretty good
shape too so he can cross it in three minutes. Gimli, being a dwarf, has stubby legs, so it will take
him five minutes, and since Gandalf is over 2000 years old, it will take him eight minutes to cross
the bridge. Whenever two of the company cross the bridge together, they must stick together
so that they both know where they are going. This entails that they move at the pace of the
slower of the two.
Is it possible for all of them to cross the bridge in 15 minutes or less? How?

