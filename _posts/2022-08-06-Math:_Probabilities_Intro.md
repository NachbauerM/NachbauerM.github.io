# Math: Learning Probabilities (Part one: Intro)

For the longest time I was under the impression that probabilities is all about throwing dice, different colour marbles, and goats beyond doors. After reading Nate Silvers´ The Signal and the Noise and getting into contact with basic statistics at work, I got a glimpse of the magic of probabilities and statistics. So let´s learn a few basics.

## Learning method

For this learning challenge I decided to try working through a textbook. I didn’t want to dive too deep into probability theory and decided to go with a statistics book: A First Course in Probability and Statistics, by Prof. Dave Goldsman (the book and additional materials can be found here: ["ISYE 6739"](https://www2.isye.gatech.edu/~sman/courses/6739/). 

## The Basics
The book starts with a definition: "Probability, roughly speaking, describes the random variation in systems, while Statistics uses sample data to draw general conclusions about a population."
Next are some prerequisites and definitions.

### Set Theory

1. A set (A, B, $\Omega$) is a collection of elements (x, y, z).
2. $\in$ means set membership. E.g. x $\in$ A means x is an element of A.
3. $\Omega$ is the universal set (a set containing all possible elements).
4. $\theta$ is an empty set (no elements at all).
Examples: B = {x $|$ -1 < x < 1} is a set of all x bigger than -1 and smaller than 1.
5. If all elements of C are also in A then C is a subset of A (C $\subset$ A). Any set is a subset of itself and the null set is also a subset of every set: $\theta \subset A \subset A \subset \Omega$ 

Cardinality of a set is the number of elements in the set $| S |$.

Complement of a Set X is a set that contains all elements not in X: $\complement(X)$ = {x $|$ x $\notin$ X}.

Intersection (and) of X and Y is a set of all elements in both sets X $\cap$ Y = ${z | z \in X and z \in Y}$. If X $\cap$ Y = $\theta$ than X and Y are disjoint or mutually exclusive.

Union (or) of X and Y is a set of all elements eigther in X or Y or both X $\cup$ Y = ${z | z \in X and or z \in Y}$.

Minus operation X - Y remove everything from X that is in Y. (= X $\cap$ Complement(Y)). 

E.g. X = {1, 2, 3, 4}, Y = {3, 4}, $\Omega$ = {1,2,3,4,5,6}: X $\cap$ Complement(Y) = {1,2}.

Symetric difference (XOR) (exclusive or) is X or Y and not both = (X-Y) $\cup$ (Y-X) = X $\Delta$ Y.

### Laws

Complements: X $\cup$ $\complement(X)$ = $\Omega$, X $\cap$ $\complement(X)$ = $\theta$

Commutative: X $\cap$ Y = Y $\cap$ X.

Associative (Order of execution does not matter): X $\cap$ (Y $\cap$ Z) = (X $\cap$ Y) v Z = X $\cap$ Y $\cap$ Z.

Distributive (X is distributed, or separately applied, to each term): X $\cap$ (Y $\cup$ Z) = (X $\cap$ Y) $\cup$ ( X $\cap$ Z)

# Experiements and Probability Spaces

Probability Space (part of an experiment) consists of:

1. A Sample Space $\Omega$
2. A set F of events (F is a set of all subsets of $\Omega$)
3. A probablity function P: F $\rightarrow$ [0, 1] that assigns probabilities to events.

(P: F $\rightarrow$ [0, 1] means a function P that takes in F and outputs [0, 1])

### Examples:
1. Toss a coin twice: $\Omega$ = {HH, HT, TH, TT} can also be = {0,1,2} for number of heads we obvserve.


## Events:
Event = a set of possible outcomes.
1. Any subset of $\Omega$
2. also $\theta$ (none of the possible outcomes observed)
3. A $\cup$ B is an event (A or B or both happen)


### Examples:
Toss three coins:
A = "exactly one T" = {HHT, HTH, THH}
B = "on Ts" = {HHH}

## Probability:
Function that maps an event A to an interval [0,1] = P(A).

Axioms:
1. O $\leq$ P(A) $\geq$ 1
2. $P(\Omega)$ = 1
3. If A and B are disjoint $(A \cap B = \theta)$ then $P(A \cup B)$ = P(A) + P(B).
=> $P(\complement(A))$ = 1 - P(A)
4. Suppose A1, A2, ... is a sequence of disjoint events: Then
$P(\bigcup_{i=1}^\infty)$ = $\sum_{i=1}^\infty$ P(Ai).


$P(A \cup B)$ = P(A) + P(B) - $P(A \cap B)$ = Venn Diagram (avoid double counting). Can be turned around depending on the data we have: P(A) = $P(A \cup B)$-P(B)+ $P(A \cap B)$

For more events think of Venn diagrams:

$P(A \cup B \cup C)$ = P(A) + P(B) + P(C)- $P(A \cap B)-$P(A \cap C) - $P(B \cap C)$ + $P(A \cap B \cap C)$

![Venn_Diagram](/images/Venn_Diagramm_1.png)


#### Probabilities to do:
1. Define Sample Space and $|$ Samples Space $|$
2. Define Event and $|$ Event $|$ (number of possibilities for that event
3. P(Event) = $|$ Event $|$ : $|$ Samples Space $|$
4. Sometimes we want $ Complement(Event) = 1 - P(Event)


## Finite Sample Space

($\Omega$) = {w1, w2,.... wn}
Event: A $\subset$ $\Omega$. P(A) = Sum of probabilities of all elements in A.

Simple Sample Space (SSS) is finite and all outcomes are equally likely: P(wn)= $1/|\Omega|$. => P(A) = (Numbers of elements in A)/(number of elements in $\Omega$).

### Examples: 
Toss a die. A = {1,2,4,6}, probability of each outcome is 1/6. sp P(A) = 4/6

## Counting Techniques (SSS)

1. If one can make choice A in n ways and B in x ways and only one choice (A or B) then we have n + b possible ways of doing so.

2. Roll two dice, how many outcomes = 6 x 6 = 36.

3. Toss n dice. There are 6^n possible outcomes.

4. Flip 3 coins = 2 x 2 x 2 = 8 possible outcomes.

5. Without replacement: E.g. pick two cards: 52 x 51.

### Permutations

Count number of ways to choose r out of n objects with regard to order.

An arragenment of n different symbols in a definite order is a permutation of the n symbols.

sequential sampling without replacement! (like how can n numbers be arranged? How can I schedule a series of n jobs? etc.)

Pn,r = n!/(n-r)!

r is the number of elements in the final tuple we want, n is the number of different symbols. (E.g. how many two digit numbers can you make from {1,2,3,4,5} = 5!/(5-2)! = 20.

### Combinations

Without regards to order! (order of members of the set has no significance).

Number of subeste with r elements out of a set of n elements.

Cn,r ("n choose r")= ${n \choose r}$ = n!/(r!(n-r)!)

${n \choose 1}$ = ${n \choose n-1}$ (e.g. ${6 \choose 1}$ = 6!/((6-1)!*1!) = 6


### Hypergeometric Distributions

Example: I have 15 red socks and 10 blue socks, I pick seven without replacement. What is the probability to pick tree red socks (and 4 blues):

tbd. markdown not working correct.

### Binomial Distributions

(with replacement, again a objects of A and b ojects of B)

Example: 15 red and 10 blue socks. Pick 7 with replacement:

P(three reds): ${7\choose 3} {15\choose 25}^3 {10\choose 25}^{7-3}$


### Multinomial Coefficients (more categories)

we have $a_i$ objects, where i = 1,2,...,c (c categories). $A = \sum_{i=1}^{c}a_i$ total number of all objects of all types. We take a sample n. What is the probability of selecting $k_i$ objects of types i = 1,2,...,c (our sample n is sum of all $k_i$) and $k_i \leq a_i$

#### Example:

I have 37 socks, 15 red, 12 green, 10 blue. I pick 9 randomly without replacement. What is the probability I get exactly 3 red, 4 green and 2 blue socks?

tbd. markdown not working correct.

### With replacement (multinomial distribution)
Generalization of binomial distribution:

$\frac{n!}{k1! k2! ... kc!}$ represents the number of ways on can chooose ki objects of categories i = 1,2...c out of total of n objects.

#### Example: 

37 socks, 15 red, 10 blue, 12 green. Randomly pick 9 with replacement. What is the probability that I get 3 red, 4 blue and 2 green?

P(3r, 4b, 2g)= ${9\choose 3,4,2} (\frac{15}{37})^3 (\frac{10}{37})^4 (\frac{15}{37})^2$


### When permutations and when combinations?

Combinations are for tuples (order doesn´t matter) and permutations for lists (order matters). Often both can be used by changning the definition for the samples space and Event.

Think of slots to distribute something. I.e. sandwich fillings: 
Slot 1 (Meat 1): Salami 

Slot 2 (Meat 2): liverwurst

= combination (order doesnt matter)

Slot 1 (Meat): Salami

Slot 2 (Cheese): Gorgonzola

= permutation (order does matter, I cant put Gorgonzonal in Slot 1 (Meat)).


# Conditional Probability and Independence

Sometimes we want to update a probability of an event as we get more information.

## Conditional Probability

P(A $|$ B) = $\frac{|A \cap B|}{|B|}$ = $\frac{P(A \cap B)}{P(B)}$ = The probability of event A given event B.

If A and B are disjoint, then P(A $\|$ B) = 0 (if B, there is no chance that A occurs).

Conditional probabilities have the same properties  as the Axioms of Probability!

### Important note: 
We can switch this equation around: E.g. 
P(B) = $\frac{P(A \cap B)}{P(A|B)}$ or $P(A \cap B)$ = P(A)*P(A|B)

### Example

Toss two dice and observe the sum. A = odd sum {3,5,7,9,11} and B:{2,3} Then:

P(A) = P(3) + P(4)...= 2/36 + 4/36 ... = 1/2

P(B) = 1/36+ 2/36 = 1/12

P(A $\|$ B) = $\frac{|A \cap B|}{|B|}$ = P(3)/P(B) = $\frac{2/36}{1/12}$ = 2/3


## Independence

Any unrelated events are independent. They are independent iff (only if):

$P(A \cap B)$ = P(A)P(B)

Events don`t have to be physically unrelated to be independent.

### Example:
Toss a die. A = {2,4,6} and B = {1,2,3,4}. Then $A \cap B$ = {2,4}, P(A) = 1/2, P(B) = 2/3 and P($A \cap  B$) = 1/3, Then P(A)*P(B) = 1/3 => A, B independent.

Independence is not the same as disjointness. If A and B are disjoint and A occurs, I know that B cannot occur. So A and B cant be independent!

Proof: A,B are disjoint $A \cap B$ = $\theta$. Then $P(A \cap B)$ = 0 < P(A)*P(B)

Independece for more than two events: a. independent from one another and b. all pairs need to be independent too!

For independent trials just multiply probabilities.


# Bayes Theorem

Allows to adjust probabilities with new information. Especially useful when we can divide samples space into distinct pices (i.e. a partition). 

Partition: of a sample space splits it into disjoint all-encompassing subsets. A1, A2, .. An form a partition of $\Omega $. 

Example: Vowels and consonants are a partition of all letters.

### Law of total Probability

This topic was hard for me to understand, fortunately I found this nice youtube video: https://www.youtube.com/watch?v=F3y8qupFfUs

If we have a partition (total sample space divided into disjoint subsets), the probability of each event is P(B) = $\sum_{i=1}^{n}P(Ai \cap B)$ (this is the part of Ai and B)

= $\sum_{i=1}^{n}P(Ai)P(B|Ai)$ (definition of conditional probability)

P(Ai)´s are called prior probabilities (before B)

P(Ai $|$ B)´s are called posterior probabilities (after B). They add up to 1.


#### Example
10 students from University A who have a 95% chance of passing an exam and 20 Students from University B who have a 50% chance of passing the exame. Pick a student randome, what is the probability he/she passes?

P(passes) = P(A)P(passes $|$ A) + P(B)P(passes $|$ G) = (1/3)(0.95)+ (2/3)(0.5)

#### Example 2

Two boxes of socks. Box A has one red and one blue sock. Box B has two red socks. Pick one at random and take a random sock out. It is read. What is the probability that thats from Box A?

R is the event that a red sock was drawn. The relevant partition is {A, B}!!

P(A $|$ R) = $\frac{P(A) P(R|A)}{P(A)P(R|A) + P(B)P(R|B)}$

= $\frac{(0.5)(0.5)}{(0.5)(0.5) + (0.5)(1.0)}$ = 1/3

In the numerator I have the probability that it is box A and the probability that the sock is red when I have box A.

In the denomintor I have all possible partitions for the sock beeing red (i.e. that it is from box A and B) and each of those probabilities.

The proability of Box A went from 0.5 (prior) to 1/3 (posterior). It was influecend by the information received. P(A) and P(B) add up to 1 (partition).

