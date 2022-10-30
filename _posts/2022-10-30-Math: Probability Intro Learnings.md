# Learnings after doing the Probability Homeworks (in progress)

In this post I want to collect some of my learnings from doing the homeworks on the first chapter of the Book "A first course in probability and statistics" (see last math post).

As expected, I found that I still lack a deeper mathematical understanding or intuition of the materials. I continue to try to identify patterns and apply simple step-by-step solutions. 
Despite that beeing suboptimal I still want to collect the mechanics/ heuristics I developed and hope to get a deeper understanding later on.

## Collection of mechanis and tricks to calculate simple probabilities:

1. Calculating the probability of "at least x happening out of y": Calculate P= 1-P(none of x happening).
2. Calculating the probability of multiple disjoint events: Sum them up!
3. Calculating the probabilities of ?? $P(A \cup P \cup L) = P(A) + P(P) + P(L) - P(A \cap P) - P(A \cap L) - P(L \cap P) +  P(A \cap B \cap C)$.
4. Calculating the probability of an event containing precisely 2 of the possible outcomes(?): $P(A \cap P \cap \overline {L}) +P(A \cap \overline {P} \cap L) + P(\overline {A}\cap P \cap L)$.
5. Binomial Distribution: requires a fixed number of Bernoulli Trials (independent experiments with a constant probability of Success/ Failure = with replacement). Formula gives respective probabilites of 0,1,2... Successes. ${number_of_trials \choose number_of_successes}  P(Success)^{number_of_successes} * P(Failure)^{number_of_total_trials - number_of_successes}$. Hint: I can define "Success differently".
6. Hypergeometric Distribution: Calculate the probability of an event consisting of multiple trials without replacement (changing probabilities after each trial): P(X = x): $\frac{{k\choose x} \cdot {{N-k}\choose{n - x}}}{N \choose n}$ N = total population, n = sample size, k = number of elements belonging to one group, x = number of "successes".
