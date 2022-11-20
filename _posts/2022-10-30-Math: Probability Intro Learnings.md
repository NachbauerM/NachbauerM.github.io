# Learnings after doing the Probability Homeworks (in progress)

In this post I want to collect some of my learnings from doing the homeworks on the first chapter of the Book "A first course in probability and statistics" (see last math post).

As expected, I found that I still lack a deeper mathematical understanding or intuition of the materials. I continue to try to identify patterns and apply simple step-by-step solutions. 
Despite that beeing suboptimal I still want to collect the mechanics/ heuristics I developed and hope to get a deeper understanding later on.

## How to structure a probability problem?
1.	Describe all possible outcomes, the sample space $\Omega$.
2.	Specify probability laws to use (describe beliefs about the outcomes of an experiment, e.g. independence, disjointness etc.)
a.	Addition rule (often when the word “or” is used in the question). Add probabilities of single Events or Elements if they are disjoint and part of one sample space (together not bigger then 1).
b.	Multiplication rule (often when the word “and” is used in the question). Multiply probabilities of Events if they are independent.
c.	Complement rule (often when the word “not” or “at least” is used in the question). Find the complement and subtract 1- complement.
d.	…
3.	Identify event of interest (try to make a picture of it, e.g. tree or Venn Diagram).
4.	Calculate.

### Discrete Uniform rule
$\Omega$ consists of a discrete amount of equally likely elements, then P(element) = 1/n. If an event K exists of K elements, then: K* 1/n or |K|/$|\Omega|$. Here we need counting rules to find |K| and $|\Omega|$.
1.	Given n objects, the number of ways of ordering them is n!
2.	Number of distinct ways of choosing k objects from n: ${n \choose k}= \frac {n!}{k!(n-k)!}$. (n choose k)

### Multiplication Rule
1.	If Events are independent: P(A and B) = P(A) x P(B)
2.	If dependent: P(A and B) = P(A) x P(A|B). I might need to do this process multiple times (break down the problem).

#### Independence
Two events are independent if P(AB) = P(A)*P(B). (Not possible to see independence in Venn Diagramms).

### Addition Rule
1.	If Events are disjoint (A and B = Empty set): P(A or B) = P(A) + P(B)
2.	If Events are not disjoint (mutually exclusive): P(A or B) = P(A) + P(B) – $P(A \cap B)$. To avoid double counting.
3.	P(A or B or C) = $P(A) + P(A^{c} \cap B) + P(A^{c} \cap B^{c} \cap C)$.

### Conditional Probability
1.	P(A|B) = $\frac {P(AB)}{P(B)}$. P(A|B)s the fraction of times A occurs among those in which B occurs as well.
2.	P(A|B) is not P(B|A)!!
3.	If A and B are independent then P(A|B) = P(A).
4.	P(AB) = P(A|B)P(B) = P(B|A) P(A)!!

### Bayes Theorem
1.	The law of total probability: Let $A_1, A_2 …$ be a partition of $\Omega$. Then, for any event B: $P(B) = \sum_{1=k}^{k} P(B|A_i) P(A_i)$.
2.	Bayes Theorem: $P(A_i|B) = \frac {P(B|A_i) P(A_i)}{\sum_{j} P(B|A_j) P(A_j)}$
3.	$P(A_i)$ is the prior probability of A and $P(A_i|B)$ is the posterior of A.

### Binomial Distribution

## Notations and Definitions:
1.	S = {w = {w1, w2….}: wi element{H,T}}, means a set S that consists of wi elements which are either H or T (“:” restricts the bigger set to some condition).
2.	$A \cap B$ or AB or (A,B) are all the same.
3.	|N| number of elements in a discrete set N.
4.	A partition of a $\Omega$ is a sequence of disjoint sets A1, A2 … such that $\bigcup_{i=1}^{\infty} A_i = \Omega$.


## Collection of mechanics and tricks to calculate simple probabilities:

1. Calculating the probability of "at least x happening out of y": Calculate P= 1-P(none of x happening).
2. Calculating the probability of multiple disjoint events: Sum them up!
3. Calculating the probabilities of ?? $P(A \cup P \cup L) = P(A) + P(P) + P(L) - P(A \cap P) - P(A \cap L) - P(L \cap P) +  P(A \cap B \cap C)$. ("Inclusion Exclusion principle").
4. Calculating the probability of an event containing precisely 2 of the possible outcomes(?): $P(A \cap P \cap \overline {L}) + P(A \cap \overline {P} \cap L) + P(\overline {A}\cap P \cap L)$.
5. Binomial Distribution: requires a fixed number of Bernoulli Trials (independent experiments with a constant probability of Success/ Failure = with replacement). Formula gives respective probabilites of 0,1,2... Successes. ${number_of_trials \choose number_of_successes}  P(Success)^{number_of_successes} * P(Failure)^{number_of_total_trials - number_of_successes}$. Hint: I can define "Success differently".
6. Hypergeometric Distribution: Calculate the probability of an event consisting of multiple trials without replacement (changing probabilities after each trial): P(X = x): $\frac{ {k\choose x} \cdot{{N-k}\choose{n - x}}}{N \choose n}$ N = total population, n = sample size, k = number of elements belonging to one group, x = number of "successes".
