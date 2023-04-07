# Math: Probabilities Counting (WIP)

The Basics of Counting are hard for me to grasp. The Textbook "Introduction to Probability" by Joseph Blitzstein and Jessica Hwang and esp. the strategic 
questions helped me to get at least a basic idea.

## Chapter One Probability and Counting (Notes)

### Sets and Stuff

- Set A or B, but not both: $(A \cap B^{c})(A^{c} \cap B)$
- Partition $A_{1}, ...., A_{n}$ are a partition of S: $A_{1} \cup .... \cup A_{n}$.

### Naive Definition

Assumpations: S needs to be finite, symentric (all outcomes equally likely) or by design (e.g. simple random sample).

### Counting

#### Multiplication Rule

Think about compound experiment (does not have to be in chronological order and also not really compound). Experiment A (e.g. kind of breads) 
has a possible outcomes and Experiment B (e.g. kind of topings) b. Then the compound experiment (Bread plus topics) has a x b possible outcomes.

Example: Tree Diagramm:

The only way for me to really grasp the bigger counting problems is by using tree diagramms. 

<img width="340" alt="image" src="https://user-images.githubusercontent.com/72666362/230676712-3f45e82c-e128-45cc-a4b8-8f0d01126718.png">

Note: It does not matter if I choose the "bread" or the "toping" first (3x2 or 2x3).
Note: A set with n elements has $2^{n}$ subsets. For each element I can choose whether to include or exclude it and multiply:

<img width="237" alt="image" src="https://user-images.githubusercontent.com/72666362/230677525-9f681a31-9670-440c-a49d-7c40caf8a105.png">
This is the same as $\sum_{k=0}^{n} {n \choose x}$

##### Sampling with replacement
Assume n objects and making k choices from them. E.g. 3 ice flavors choosing 2 times = 3 x 3 or $3^{2}$. Order matters (e.g. chocolate then vanila is one outcome 
and vanila and then chocolate is another outcome)!! Ajust for overcounting.


##### Sampling without replacement
Then there are: n x (x-1) x (n-2).... x (n-k + 1) outcomes.
<img width="326" alt="image" src="https://user-images.githubusercontent.com/72666362/230679349-27a505f9-0278-4dc6-9e3e-601783558566.png">


### Tips
- Sometimes finding the complement is easier (e.g. for problems that ask for "at least xx").
- 

