# Qualification-Round-2021
code jam 2021 Qualification Round 2021 solution

Problem
Note: The main parts of the statements of the problems "Reversort" and "Reversort Engineering" are identical, except for the last paragraph. The problems can otherwise be solved independently.

Reversort is an algorithm to sort a list of distinct integers in increasing order. The algorithm is based on the "Reverse" operation. Each application of this operation reverses the order of some contiguous part of the list.

Problem
Cody-Jamal is working on his latest piece of abstract art: a mural consisting of a row of waning moons and closed umbrellas. Unfortunately, greedy copyright trolls are claiming that waning moons look like an uppercase C and closed umbrellas look like a J, and they have a copyright on CJ and JC. Therefore, for each time CJ appears in the mural, Cody-Jamal must pay X, and for each time JC appears in the mural, he must pay Y.



Cody-Jamal is unwilling to let them compromise his art, so he will not change anything already painted. He decided, however, that the empty spaces he still has could be filled strategically, to minimize the copyright expenses.

For example, if CJ?CC? represents the current state of the mural, with C representing a waning moon, J representing a closed umbrella, and ? representing a space that still needs to be painted with either a waning moon or a closed umbrella, he could finish the mural as CJCCCC, CJCCCJ, CJJCCC, or CJJCCJ. The first and third options would require paying X+Y in copyrights, while the second and fourth would require paying 2⋅X+Y.

Given the costs X and Y and a string representing the current state of the mural, how much does Cody-Jamal need to pay in copyrights if he finishes his mural in a way that minimizes that cost?

Problem
Note: The main parts of the statements of the problems "Reversort" and "Reversort Engineering" are identical, except for the last paragraph. The problems can otherwise be solved independently.

Reversort is an algorithm to sort a list of distinct integers in increasing order. The algorithm is based on the "Reverse" operation. Each application of this operation reverses the order of some contiguous part of the list.

Problem
You want to sort N distinct items, x1,x2,…,xN. Unfortunately, you do not have a way of comparing two of these items. You only have a way to, given three of them, find out which one is the median, that is, which one is neither the minimum nor the maximum among the three.

For example, suppose N=5 and you know that:

x1 is the median of {x1,x2,x3}
x2 is the median of {x2,x3,x4}
x3 is the median of {x3,x4,x5}
Then, it is guaranteed that the sorted order of the elements is either x4,x2,x1,x3,x5 or its reverse x5,x3,x1,x2,x4. Notice that by knowing only medians, it is impossible to distinguish the order of any list from its reverse, since the median question has the same result for any three elements in both cases.

Your program will have to find the order of T lists of N elements using at most Q median questions in total (or Q/T queries per list on average). In each case, finding either the right order or its reverse is considered correct. The order for each case is generated uniformly at random from all possible orders, and independently of any other information.

Problem
100 players are competing in a 10000-question trivia tournament; the players are numbered from 1 to 100. Player i has a skill level of Si and question j has a difficulty level of Qj. Each skill level and each question difficulty are chosen uniformly at random from the range [−3.00,3.00], and independently of all other choices. For example, a player can have a skill level of 2.47853 and a question can have a difficulty level of −1.4172.

When player i tries to answer question j, the probability that they answer it correctly is f(Si−Qj), where f is the sigmoid function:
f(x)=11+e−x
where e is Euler's number (approximately 2.718...), the mathematical constant. Notice that 0<f(x)<1 for all x, so f(Si−Qj) is always a valid probability. Each of these answer attempts is chosen at random independently of all other choices.

There is one exception: exactly one of the players is a cheater! The cheater is chosen uniformly at random from among all players, and independently of all other choices. The cheater behaves as follows: before answering each question, they flip a fair coin. If it comes up heads, they do not cheat and the rules work as normal. If it comes up tails, they secretly look up the answer on the Internet and answer the question correctly. Formally, they decide whether to cheat at random with 0.5 probability for each question, independently of all other choices.

The results of a tournament consist of only the per-question results (correct or incorrect) for each player. Apart from the general description above, you do not know anything about the skill levels of the players or the difficulties of the questions.

You must correctly identify the cheater in at least P percent of the test cases. That is, you must succeed in at least P⋅T/100 out of T cases.
