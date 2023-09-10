# Online_Course: Rigorous_Impact_Evaluation (MIT)

Rigorous Impact Evaluations (RIE) have become a trendy topic in development cooperation. To get a better idea of the area I took the MOOC “Evaluating Social Programs” on MITx Online. The course contents were excellent for someone newish to the topic like myself. The course has 10 chapters.

## Why evaluate?
Each policy challenge has many potential solutions, but limited funding and time. How do we know if a chosen program really works.

Definition Impact: Difference in outcome after an intervention compared to a counterfactual.
 
The problem: Counterfactuals are impossible to get. 
Solution: Mimic counterfactual via an RIE.

Randomized Control Trial (RCT): 
1.	Identify all eligible participants
2.	Random lottery (treatment group, comparison group)
3.	Measure outcomes for both groups (on average both groups are similar)
Prerequisites:
1.	Needs assessment is necessary (What is the problem? What are underlying sources of the problem?)
2.	Design program and theory of change (need, input, output, intermediate outcomes, final outcomes)
3.	Process evaluation (during implementation, is the program implemented as planned e.g. is the treatment group getting the service and the comparison group not? Was the intervention delivered as intended?)
4.	Estimate impact (how big and if at all)
5.	Conduct a cost-effectiveness analysis (how does the programs effectives compare to others). CEA! Is the program worth for a scaled role out?

Example Evaluations can be found here: Evaluations | The Abdul Latif Jameel Poverty Action Lab

## Theory of Change and Measurement
KEY VOCABULARY
Theory of Change	Describes how and why a desired change is expected to happen. The theory of change identifies the preconditions, pathways, and interventions necessary for success.
Hypothesis1
A prediction about the effects of a given intervention, often derived from a theory of change. We can think of this as a claim to be tested. Hypotheses are intended to be made prior to the implementation of the intervention. E.g., Giving textbooks to students will improve student learning.
Assumption	A precondition that underpins a theory of change or model. An assumption cannot be directly observed or verified, e.g., When students read textbooks, they learn from them.
Input	An activity carried out as part of a program or intervention, e.g., Textbooks are given to schools.
Output	A step in the planned implementation of a program or intervention – a.k.a. a direct result in response to the inputs, e.g., Students receive textbooks through schools.
Outcome	A change or impact caused by the program that is being evaluated, e.g., Increase in student learning levels.
Intermediate Outcomes	Observable changes or impacts caused by the program that are not the ultimate outcome of interest, but necessary along the way to achieving a final outcome, e.g., Increase in students who have passing test scores for the semester.
Final Outcomes	Changes or impacts that are of ultimate interest to researchers and/or program implementers; these are often the overall goals of a program, e.g., Increase in high school graduation rates.
Indicator	An observable metric used to measure an outcome, e.g., Student test scores.
Instrument	The tool used to measure an indicator, e.g., A set of test questions

Interesting: implicit association tests IAT (online test). Puts groups of categories together and check associations (we are faster if associations fit our intuitions). Tests implicit discrimination.

Accuracy (Validity): Am I measuring what I want to measure? How well does the indicator map to the outcome? Are survey questions unbiased?
Different Biases that influence measurements: 
•	People tell us what they think we want to hear (demand bias, response bias).
•	They want to appear as a good person (social desirability bias).
•	Frame around a question is important (Framing effects).
•	Recall bias (consistency bias): Hard to recall past information correctly.
•	Anchoring bias (dont add anchors in questions)
Precision (Reliability): How precise is my measurement? Is that a good way to get the data ? How consistent and precise is the measure? In Practice:
- Length, fatigue
- Ambiguous wording
- Answer choices (open/ closed, Likert scale e.g. 0-7, ranked)
General Noise: surveyor training, poor translation, data entry,
Hard to measure:
-	Things people don’t want to talk about (sex, mental health, violence; anonymize, ask third person questions, safe atmosphere)
-	Things people don’t know well. (estimates esp. across time see recall error; integrate consistency checks)
-	Things that are not directly observable
-	Things that are best directly observed.
-	…
Ressources: Survey design, Repository of measurement and survey design resources 
## Why we randomize?
Before-after-Analysis doesn’t work. Outcomes might have been due to other influences. Only the difference between the counterfactual and the measured outcome is the impact.

Other impact evaluation methods: Pre-test, simple difference, differences-in-differences, multivariate regression, statistical matching, interrupted time series, instrumental variable, regression discontinuity.

RCT is the gold standard. No need to artificially/ statistically account for differences in control and treatment group.
Key steps for an RCT:
1.	Design study carefully
2.	Randomly assign people to treatment and control.
3.	Collect baseline data (increase statistical power, find issues with random assignment).
4.	Verify that assignment looks random (key averages).
5.	Monitor process (give the control group a placebo if possible, to account for the placebo effect).
6.	Collect follow-up data for both groups.
7.	Estimate the program impact by comparing the mean outcomes of control and treatment group.
8.	Assess if the program impacts are significant.

Omitted Variable Bias	Statistical bias that occurs when relevant (and often unobservable) variables/ characteristics are left out of the analysis. When these variables are correlated with both the primary outcome and a variable of interest (e.g., participation in an intervention), their omission can lead to incorrectly attributing the measured impact solely to the program. For example, omitting socioeconomic status, which is correlated with test scores, could lead to overestimating the impact of a tutoring intervention on a group of wealthy students
Selection Bias
	Selection bias occurs when individuals who receive or opt into the program are systematically different from those who do not. Consider an elective after school tutoring program. Is it effective at raising children’s exam scores? If we compare those who take up the tutoring program to those who don’t, we will get a biased estimate of the effect of the tutoring program, because those who chose to take it up are likely different from those who don’t. The two groups likely are not balanced (for example, those who took it up may be more motivated, or they may have lower grades). Randomization minimizes selection bias because it breaks the link between characteristics of the individual and their treatment status. Selection bias can occur in other ways in a randomized evaluation. For example, participants can choose to take up a treatment or refuse it, and participants can choose to leave the study (i.e., attrit/attrition).



## How to randomize?
Units of randomization (clusters, municipality, school, village, city, family  or individuals). Ask if the program is designed to deliver to individuals or institutions. 
How to choose:
1.	How the intervention is administered?
2.	Power requirements (sample size)
3.	Aggregation level of available data
### Simple lottery
Have a random process selecting participants from a fixed list.
### Randomizing in the bubble (partial lottery, restrict sample)
Do a screening of all potential participants. Restrict the sample for randomization to those people who are just on the edge of meeting a certain criterion of eligibility. E.g. below a test score of 600 and above a test score of 300.
### Phase in Design
Start the intervention with the treatment group and give the control groups intervention later (everyone gets the intervention in the end). Problem: in the end of the last phase, we don’t have a control group anymore (e.g. measure long term effects).
### Rotation Design
One group gets the treatment one year and the next one the next year. And then swap again.
Risk: treatment groups can change because some group gets something (e.g. because of free school food). Think about knock-on effects!! Difficult to measure long term effects.
### Challenges
1.	Often people in the control group don’t want to fill out surveys.
2.	Sometimes its hard to separate between units of intervention (what is a village?). Ask people about their preferred definition.
### Constraints
1.	Political constraints: Partner wants something that is not compatible with the RIE. E.g. wants to select certain areas of implementation. Potential to drop these observation and randomize/evaluate the rest.
2.	Spillovers: Effects that come from the randomization process and influence the impact of the project. Spillovers because interventions might get shared between the groups (e.g. information).
3.	Logistical issues: Hard to maintain a strict separation between control and treatment group (e.g. health workers cant deny an intervention).
4.	Sample size: Issues with statistical power. Sample needs to be big enough.
### Intent-to-treat estimate
Calculated by comparing everyone in the control group to everyone in the treatment group. No matter if they took up the intervention or not. A randomized selection process ensures that the intent-to-treat estimate is an unbiased estimate of the average treatment effect because there are no systematic differences between the treatment and comparison groups.

### Multiple Treatments
With a large enough sample (esp. if effect size is estimated to be small) we can test multiple treatments.
Find out diminishing returns, cost effectiveness etc.
-	One group gets treatment A 
-	One group gets treatment B
-	One group gets treatment A and B.
Or:
-	One group gets only 50% of threatment
-	One gets 100% 
-	Find if we have diminishing returns.
### Stratification
The statistical power for small random samples
Stratification: Take all e.g. boys in one group and all girls in another. Then choose randomly from within both groups (same amount). Can use more variables (on a computer).
When to do this: 
1.	Small sample
2.	Good theory of which strata are important (guessing)
3.	When we are interested in effect on a particular sub-group.
4.	When we have good data about the target.
5.	When we have old data about some effect for some variables and use those to predict the new interventions outcome (stratify for those variables that where important in the old data).
Vocabulary:
Unit of randomization: level of observation (individual, village, school) at which treatment and control are randomly assigned.
Factorial design: evaluation design that tests different treatment in different combinations (cross-cutting design) to determine how they work separately vs. in combination.
Stratification: dividing units in your sample into different subgroups based on specific characteristics. Then randomizing within those groups to ensure balance on these characteristics.

## Statistics Review (Sampling and Sample dice)
Basic question: How confident can we be in our results?
## Law of large numbers: If we increase the number of independent times we do an action, most averages we get will get closer to the true average (expected average). E.g. rolling 100 dice the average will be very close to the true average of 3.5
## Central limit theorem: describes the behavior of the distribution of sample means. It states that if you have a population with mean μ and standard deviation σ and take sufficiently large random samples from the population with replacement, then the distribution of the sample means will be approximately normally distributed.
For instance, let’s say you roll the two dice 10 times and record the sum for each roll. You then calculate the average of these 10 sums. This is one sample mean. If you repeat this process many times (e.g., 1000 times), calculating a new sample mean each time, then the distribution of these 1000 sample means will be approximately normal.
If we take a sample out of the underlying population and this sample is big enough, the average is likely to be close to the true average. If I take multiple samples, their averages will be normally distributed around the true average.

Each item is the average test score of the 10 students drawn.








### Accuracy and Precision
Accuracy: Average of results is close to the accurate answer (randomization, answers we get are closer to the truth). Accuracy is more important (precision of a wrong thing is bad).
Precision: low variance results (Sample size increases precision, law of large numbers).
### Standard error
It is used to estimate the variability of the statistic if the sampling process were repeated many times. The standard error is estimated by dividing the standard deviation of the sample by the square root of the sample size. (This means since the sample size is square rooted the decrease in the standard error are not linear with increasing the sample size).
The standard error gives us an idea of how much variability we can expect in our sample means if we were to repeat this process many times. It is a useful tool for understanding how well our sample represents the population and for making inferences about population means using sample means.

##Standard deviation
Measure on how dispersed the population is around the mean. 1 standard deviation away means (mean + and – the standard deviation e.g. mean is 10, STD = 5; 1 standard deviation away is range between 5-15).
# Statistical Significance
## Hypothesis testing
Presumption: start with the “null hypothesis” (assume no effect of a program, represented by the control group). Can we now present enough proof that our observations is sufficiently unlikely if we had no effect to happen from chance? 
Definition: Statistical Significance = if the probability of getting our result (impact) by random chance is less than 5%, we say something is statistically significant (we reject the null hypothesis).
Type 1 error: rejecting the null hypothesis even though it is true (false positive).
Type 2 error: accepting the null hypothesis even though it is false (false negative)
Both depend on our definition of statistical significance.

## Statistical Power
Power: Statistical power is the likelihood that a statistical test will detect an effect if there is one. It is the probability of correctly rejecting the null hypothesis when it is false. For example, if a study has an 80% power, it means that the study has an 80% chance of detecting a significant effect if there is one.
Statistical significant if we can reject null hypothesis with 95% probability. 
In the picture: blue is null hypothesis, red is the results if we did it very often. Statistical significant only if probability that the effect is part of the null hypothesis graphs is less then 5 percent (cutoff). Power is the part (%) of the red curve that is beyond the cut of)


Increasing the Power: 
The bigger the effect (effect size) the more power (more away from the null hypothesis).
Or if I increase sample (the bell curve will get less wide and make the bell curve of the effect and the null hypothesis less overlap). Clustering (-	Low intra-cluster correlation (Rho) necessary), Proportion of sample in Treatment vs. Control can increase the power.

Always ask what the probability is of getting a certain value if the null hypothesis was true. (basis hypothesis testing).

### Effect Size 
Effect Size: is a statistical concept that measures the magnitude of the difference between two groups.
Calculate: Cohen’s d is a statistical measure that is used to indicate the standardized difference between two means. It is commonly used to determine the effect size of an intervention or treatment in experiments, by comparing the means of a treatment group and a control group. Cohen’s d is calculated by taking the difference between the two means and dividing it by the pooled standard deviation (weighted average depending on the sample size of both SDs) of the two groups. The resulting value represents the difference between the two means in terms of standard deviation units
Makes a big difference regarding Power (how many SD is the effect result mean away from the null hypothesis).
-	Effect size is influenced e.g. by take up rate (e.g. we expect an effect of 3 and only 1/3 of the people in the treatment group take it, the effect size is 3*1/3). I would need to increase the sample size by 9 to get the same power.
-	It is thus important to decide up front what the smallest effect that you care about is, and to then design your experiment to be sufficiently powered to detect effects at least as small as that size. Note that the study would by design be powered to detect larger effect sizes than your minimum detectable effect size (since the larger the effect, the higher the power that you have with a given sample size.)

### Sample Size:
-	Increase precision. Makes both distributions more precise.
 


## Tutorial on Sample Size and Power
Do a power calculation before the study is done:
-	Determining the approximate number of units (people, households, schools) needed to detect a given effect.
-	Deciding whether to go ahead with the study or not, especially when the cost associated is high.
-	Understanding how different design choices, such as choosing which unit to randomize at, affect power.

“Power calculations” refers to an exercise of determining which combinations of parameter values (related to the components of power you were introduced to in the lecture) will ensure a certain level of power in your study (typically 80%). Done by:
-	Determining the sample size that ensures a power of 80% for a given set of parameters, including the minimum effect size you expect the program to have
-	Determining the minimum effect size required to achieve 80% power for a given set of parameters, including the sample size. This is called the minimum detectable effect (MDE ).
Formula (there are calculators for that online Power Calculator (shinyapps.io)):
 
The paradox of power calculations is that some parameters—e.g., the effect size and the variance of the outcome of interest—will not become known until the experiment has been conducted.
In this regard, power calculations involve making careful assumptions about certain outcomes, such as the effect you realistically expect your program may have or the variation you expect in the outcome variable. These assumptions are often informed by real data, such as from previous studies. Regardless of the source of the data you use to inform your power calculations, it is important to justify your assumptions, which requires carefully thinking through the details of your program and context.
Consider the following parameters and determine what values are reasonable for each of them:
-	Effect size: The smallest effect size that is expected and/or is policy-relevant
-	Take-up rate: The proportion of participants in the treatment group who take up the intervention
-	Sample size: The maximum sample size realistically possible. In a clustered design, this includes determining both the maximum number of clusters and units within clusters
-	Attrition rate: The proportion of participants for whom endline data cannot be collected
-	Variance: The underlying distribution of the outcome of interest before the intervention
-	Intra-cluster correlation coefficient (for cluster randomized studies): The level of correlation/similarity between units within a cluster

As a starting point, I can calculate power for a “best case” and a “worst case” scenario. If the required sample size for the “best case” scenario is much above what I think is reasonable to recruit, I might want to consider whether an RCT is the best method of evaluation. If, on the other hand, the required sample size is reasonable, I can conduct sensitivity analyses, which involve testing how power changes with changes to critical assumptions.

The minimum detectable effect size entered into your power calculations should be the minimum expected effect size for those taking up the program adjusted by the take-up rate. For example, if you expect the effect size to be 10 percentage points among the people who take up the program, but you expect that only 80% of the treatment group will take up the program, the effective effect size will be 10 percentage points times 0.8 = 8 percentage points. Thus, the study should be able to detect a minimum effect of 8 percentage points, meaning that the MDE entered into the power calculations should be equal to or smaller than 0.8. Because the effect size involved in power calculations is scaled by the take-up rate, improving the take-up rate (as well as ensuring that people in the comparison group do not take up the treatment) is one of the most effective ways of improving power.
Vocabulary:
Type I error	A false positive: falsely concluding that the program/treatment had an effect when it actually did not.
Significance level (α)	The maximal probability of committing a type I error we want to allow. Statistical tests are typically performed at significance levels of 1%, 5%, or sometimes 10% to determine whether one group (e.g., the treatment group) is different from another group (e.g., the comparison group) on certain outcome indicators of interest (for instance, test scores in an education program). The significance level is typically denoted by alpha (α).
Type II error	A false negative: The probability of falsely concluding that there is no treatment effect.
Power	The likelihood of avoiding a type II error, that is, the probability that your statistical test will distinguish the program effect (correctly) from zero when the program/treatment actually has an effect.
Unit of randomization	The level of observation (e.g., individual, household, school, village) at which treatment and comparison groups are randomly assigned.
Sample size (N)	The total number of units in the study, in both treatment and comparison groups. In a clustered randomization, the sample size is the total number of units across clusters. The power increases with the sample size with everything else remaining constant.
Minimum Detectable Effect (MDE)	The effect size is the difference between the average of the outcome of interest in the treatment and control groups. The MDE is the minimum effect size that can be detected with given statistical power (probability of correct positive, e.g., 80%), statistical significance (probability of a false positive, e.g., 5%), and sample size N. All else equal, the smaller the effect, the larger the sample size required to detect that effect.
Variance/Standard deviation	This is the measure of the spread of a sample or population for a particular indicator. Mathematically, the standard deviation is the square root of the variance. Given a sample size and effect, the power of the study decreases if the outcome variable has a higher variance.
Cluster	The unit level at which a sample is randomized (e.g., school), each of which typically contains several units of observation that are measured (e.g., students). Generally, observations within the same unit of randomization that are potentially correlated with each other should be clustered, and the required sample size should be calculated with an adjustment for clustering.
Intra-cluster correlation coefficient (ICC)	The ICC describes how similar or correlated units within a same class or cluster are. For instance, if your experiment is clustered at the school level and the outcome of interest is test scores, the ICC would be the level of correlation in test scores for children in a given school relative to the overall distribution of test scores of students in all schools. The ICC is often denoted by rho (ρ).
Treatment allocation	The proportion of the sample assigned to the treatment group. Power is typically maximized with an equal split between treatment arms

## Threats and Analysis: What can go wrong?

### Attrition (people disappear from the sample): 
to compensate for 50% attrition, we would need to double the sample to have similar statistical power. Risk that there is a bias with the people not responding (if the type of people who disappear is correlated with the treatment).

How can we solve attrition bias: 
-	Devote resources to track participants after they leave the program. Get as much information about the beneficiaries as possible (phone, email, phone of family members etc.).
-	Pay participants to stay (incentives)
-	Check if attrition affects the same kind of people in treatment and in control.
-	Try to bound the extend of the bias (fill in missing data with worst case scenario, e.g. all in control group changed and no one in treatment group, then the other way around, re-estimate effect both times, gives a bound for the effect size between the two). Imputation of missing data.

### Spillovers
Sometimes people from the control group take the treatment as well (e.g. vaccine half the population this might effect the control group if they are in contact, get it from elsewhere).
-	Sometimes we are interested in knowing spillover effects (make multiple groups and each gets a different level of intervention e.g. vaccines, check size of spillovers)

### Partial compliance and sample selection bias
Treatment group members don’t show up. And/ or control group people cross over (Spillover). 
In the case of partial compliance, we can calculate the intent-to-treat estimate or the difference between the means in the treatment and control groups. This is an estimate of the effect of the program on those assigned to treatment, regardless of their take-up.
Intention to treat (ITT): Mean of the treatment group- mean of the control group. (often policy relevant since most programs have limited compliance and this gives the policy maker a good idea of the cost benefits of a program). Still, we don’t get the actual effect of the measure (exact effect).
Treatment on the treated (TOT): tells us about the effect on those who took up the treatment because they were assigned to the treatment. We are not estimating the effect on the control group members who did not comply with the assignment.
-	need the average of the treatment group (Y(T)) 
-	the average in the control group (Y(C)), 
-	Probability of getting treated in treatment group P [treated|T]
-	Probability of getting treated in control group P [treated|C]
-	TOT = (Y(T)- (Y(C)), /(P [treated|T]- P [treated|C])
For that to work we need a considerable impact. P [treated|T]-should be very high and P [treated|C] should be very low.

### Can we look at various outcomes:
The more outcomes we look at, the higher the chance to find a least one significantly affected by the program (by chance) => Pre-specify outcomes of interest., report results of all measured outcomes.

### Include covariates.
Control for gender, age etc…. May explain variation. But can also be used to manufacture a result (which came by chance). Always report raw differences as well. Define it advance what covariates to use.

### External validity
Being in an evaluation can change behavior: in control and/or treatment.: minimize salience of evaluation as much as possible. Consider including controls who are measured at the end-line only. “Hawthorne effect”: people change behavior if we are observed (treatment). “John Henry effect”: work harder because you are in the control.
Generalizability: representativeness of the study sample/ can it be scaled? Sensitivity of results (would a similar program have the same or bigger impact?). This is an issue with all evaluation methods though.

Key Vocabulary
Treatment assignment and treatment status	An individual’s treatment assignment is the group they were randomly assigned to, either a treatment or comparison group. An individual’s treatment status is what actually happened to them, whether they were treated or not, and the kind of treatment. 
Balance	Randomization creates two groups that on average look very similar. This can be tested for observable characteristics by collecting some baseline demographic information—such as age, gender, years of education, income, etc.—and comparing the average value of these characteristics in the treatment group to the average value of them in the comparison group. Even when randomization is done correctly, some of these average values may differ due to random chance. We say the comparison and treatment groups balance if they have similar average values for observable baseline characteristics.
Selection Bias	Selection bias occurs when individuals who receive or opt into the program are systematically different from those who do not. Consider an elective after-school tutoring program. Is it effective at raising children’s exam scores? If we compare those who take up the tutoring program to those who don’t, we will get a biased estimate of the effect of the tutoring program, because those who chose to take it up are likely different from those who don’t. The two groups likely are not balanced on key characteristics (for example, those who took it up may be more motivated, or they may have lower grades). Randomization minimizes selection bias because it breaks the link between the characteristics of the individual and their treatment status. Selection bias can occur in other ways in a randomized evaluation. For example:
•	Participants can choose to take up a treatment or refuse it
•	Participants can choose to leave the study
Attrition Bias	Attrition bias is a type of selection bias that occurs when people leave the study. This can bias the estimate of the treatment impact in two ways:
1.	It may be the case that people with certain characteristics (say, those with the highest levels of education) in both the treatment and comparison groups leave. This means your study population looks less like the general population. The treatment effect you estimate might not represent the true effect for the general population.
2.	The reasons people leave may be correlated with the treatment. Suppose that students who have the most resources at home and are in the treatment group improve their performance and test into elite private schools, leaving your study sample. Then comparing treatment and comparison groups after the program would underestimate the impact of the program, because the students with the highest grades are ‘missing’ from the treatment group.
Spillovers	Spillovers mean that the outcomes of untreated units are indirectly affected by the treatment given to others. Spillovers can be positive or negative.
Compliance	When a unit's treatment assignment (assigned to treatment or comparison group) matches their treatment status (took up or did not take up the treatment), we say they have complied.
Any study sample can be split into three distinct groups:
•	Compliers:  This group of people will follow their assignment status. If they are assigned to the treatment group, they will take up the treatment; if they are assigned to the comparison group they will not take up the program.
•	Always-takers: This group of people will always take up the program, regardless of assignment status.
•	Never-takers: This group of people will never take up the program, regardless of assignment status.
When respondents do not comply with their treatment assignment, the study has partial compliance. In the treatment group, the people who do not comply are never-takers, while in the comparison group, those who do not comply are always-takers. We collectively refer to those who do not comply as non-compliers and the action of not complying with treatment status as non-compliance.
Note that when there is two-sided non-compliance (i.e., non-compliance in both the treatment and comparison group), we have to make the monotonicity assumption, which states that assignment to treatment does not dissuade someone from taking up the treatment (in which case, we would classify them as “defiers”).
Intention-to-Treat (ITT)	The ITT is a method for estimating the effect of the program where you compare the average outcomes of those assigned to the treatment group to the average outcomes of those assigned to the comparison group, regardless of whether individuals within those groups have actually received the treatment. The ITT measures the impact of delivering a program in the real world, where some people don’t take up the program when offered it, and others take up the program even when they are not expressly encouraged to do so.
Local Average Treatment Effect (LATE)	The LATE is a method for estimating the effect of the program on those who complied with their treatment status. The LATE divides the ITT by the difference in the proportion of the treatment group who took up the program and the proportion of the comparison group who took up the program. Recall that the ITT compares the average outcome of the treatment group to that of the comparison group. This means that under partial compliance, the average changes we measure in the treatment group will be diluted by changes in outcomes among those who did not take it up. Intuitively, you should think of the LATE as a way of adjusting the ITT to reflect that not all of those assigned to treatment were treated while some who were assigned to the comparison group were treated. LATE is sometimes referred to as Complier Average Treatment Effect (CACE). 

## Ethics
Ethical rules (framework) for research with human subjects:
•	Respect for person (inform participants of the risks, should have a true choice in joining the study)
•	Beneficences (balance risks of research vs benefits)
•	Justice (people who take the risk with the research should also the ones who benefit).
### Benefice 
-	Minimize risks, maximize benefits (credible, accessible and actionable findings)
-	Do not withhold a benefit that would otherwise be available (e.g. phase-in design)
-	Some risk is acceptable if balanced by potential benefits.
-	Do fewer people receive the program because of the evaluation (e.g. if we know the benefits of a program).
-	Do different people receive the program because of the evaluation? E.g. we know the program would help very malnourished people and we still give it to others as well to evaluate.
-	Risk of data becoming public
### Justice
Test in the place (and with the same people) where we want to scale it up. Don’t exclude certain subpopulations (e.g. historic exclusion of, esp. pregnant, women in medical trials). Test on the whole range of people.
### Institutional Research Board
Everyone involved in the research needs to know the ethical considerations (trainings, should be documented). Review and approval of surveys and consent forms. Data management plan. Annual updates on the status. 
Personally identifiable information (PII): names, geographic info, telephone numbers, combination of information (e.g. village and occupations). Secure data management system.
Plan for IRB approval and plan time for it. Don’t start without it.

## Cost Effectiveness and Scaling up
Value for money! Cost-effectiveness analysis (CEA) summarizes complex programs in terms of a simple ratio of costs to impacts and allows us to use this common measure to compare different programs evaluated in different countries in different years. 
CEA: Is the ratio of the costs of a program to the effects it has on one outcome. 
CEA can sometimes compare across programs (e.g. compare deworming, information, school uniforms, scholarships on years of schooling). => important to compute costs and benefits using similar methodologies.
Cost-Benefit Analysis: include more outcomes (e.g. deworming: schooling, health, future labor market value etc.). Lots of assumptions are necessary though (little less transparent than Cost-Effectiveness analysis.
When is it useful? 
-	Have multiple options to choose from
-	Convince decision makers of a non-conventional program.
-	To make inferences by changing the assumptions of the CEA (e.g. how much would it cost if we buy on a larger scale? Etc.)
What do we need?
-	Impact measure from the RIE
-	Costs data: need fairly disaggregated specific data on costs.
Challenges: 
-	Often an absence of incentives to do CEA.
-	Not straight forward (multiple outcomes, spillovers etc.)
-	Costs are hard to gather 
Use Ingredients method https://www.povertyactionlab.org/sites/default/files/research-resources/costing-guidelines.pdf: 
-	Collect costs directly connected (ingredients) needed for the program. Try and find the costs for the items (also public sources, estimates etc.).
-	Do it prospectively: Define ahead of the program which costs we want to include and keep track of them!!

### Sensitivity Analysis: 
Modifying assumptions and local conditions for policy makers (e.g. assume different price for an ingredient etc.). Account for exchange rates, inflation, multiple outcomes, present vs. future value if programs are compared.
### Scale up: 
After a RIE and Cost effectiveness analysis: Ideally pilot before scaling in another context (ideally, partnerships building, dissemination, policy outreach). Often differences in: Spillover effects, costs of inputs might change, hard to control local differences (prices, motivation, political decisions), partial vs. general equilibrium (e.g. job trainings good effect on small scale, but on national scale reaching an equilibrium).

## Generalizability
General lessons generalize better.
We are not aiming for 100% certainty, when we give policy advice. Combine it with local knowledge and other evidence. Never look at a single study in isolation!!! Weight different kinds of evidence to come up with a conclusion.
How to do this (assess evidence):
-	Need a theory of change. Check each step of the theory of change in new context (do basic assumptions hold in other context?). Do basic conditions hold locally? 
-	Evidence on process of the implementation. Check how similar the process for implementation would be. Will a process work in another context? (e.g. logistics, technicalities etc.) Adapt those if necessary (or do a logistical pilot).
-	Do underlying behavior issues hold locally (check other studies on these issues). E.g. many studies that also small incentives have a big effect on compliance.
-	Meta analysis can help (averaging over the impact coefficients might lose context if done over generally). Still need a theory-based approach to that. Otherwise miss context, covariants, etc. Literature reviews can also help.
Conclusion:
-	Do RCTs replicate in other contexts? Too big of a question. Break down the theory of chain to see if the initial assumptions hold in the new context. Do the local conditions hold? How strong is the evidence for the general behavior change (are there multiple RCTs)? What is the implementation process (can we replicate the intervention)?
-	Sometimes we need more information (esp. if the intervention is important or costly or not well researched). Sometimes we need to act on incomplete information (better than nothing).
-	“Making things actually just work in the development context is usually 90% of the work.”

Overview: https://ssir.org/articles/entry/the_generalizability_puzzle

## RCT from Start to finish
1.	Think long and early about what questions to answer.
2.	Get good partnership between evaluators and implementers (good communication).
3.	Create Theories of Change (also include impacts on the overall population, e.g. negative effects of supporting the establishment of new businesses for already established businesses).
4.	Create Log Frame from that (Outcomes, Ouputs, Activities), Indicators, Sources of verification, Assumptions and threats. Measuring multiple indicators is possible if the Sample is big enough.
5.	Formulate additional research questions based on that (e.g. check assumptions, other outcomes).
6.	Measurements (Indicators): often very hard to attain e.g. through household surveys (solution e.g. walk people through a survey). Worry for strategic answering (assume under or overreporting is similar in treatment and control group).
Study design:
1.	Randomization (what unit to randomize at): often problems with the design of the intervention. If the sample is small we need a very big effect size to get more power. Individual, group, service provider, neighborhood (something people identify with) communities, villages, areas…
2.	Randomization on the fly is possible (e.g. 6 come in we take 3 in control and 3 in treatment, then the next group comes, do some stratification if possible). Take care of spillover effects (e.g. make bigger units if possible).
3.	Often gets messy. E.g. suddenly a new micro finance company comes into comparison and/or control groups.
4.	Can still do analysis on another level unit of analysis): unit of analysis is the level at which the outcomes are measured and compared across treatment and control groups. It may not always be the same as the "unit of randomization".
Threats: Low take up. Ensure compliance with the research design (implementer). Other actors do something similar in the control groups.
Endline survey: Use information from the baseline to compare within control and treatment group. E.g. women who have a business and women who are likely to start a business (effect of microloans on those), by using data from the baseline. Compare always these subgroups between control and treatment. Or if we don’t have the baseline data, project from the endline (e.g. Age or situation of older children does not change because of the intervention).
The development community often makes very big claims (raises expectations unnecessarily).

