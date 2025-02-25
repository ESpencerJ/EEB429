# Assignments for class
Written below are the assignment details for the individual assignments to provide context for the purpose of the code.

## Intro to Probability 1: Assignment
Due by the beginning of class next Tuesday
Save this Rmarkdown script as a file named “YourlastName_Assignment12.Rmd”. For each question, fill out the answer and, where requested, provide the relevant R code using “```” and the echo = TRUE argument.

When finished, Knit your script together into an html report, saved as “YourlastName_Assignment12.html” and upload the resulting file to Canvas to turn it in.



This homework assignment will test your abilities to:

think critically and creatively about probability

use simulations to build intuition

use your R skillz: function building, data visualization, etc.



Question 1
Define the following terms:

probability

simple event

complex event

shared event

conditional probability

statistical independence

Question 2
Suppose you have a fair six-sided dice (“fair” meaning that the probability of rolling any number is equal) and a fair coin (p(heads)=p(tails)). Suppose you roll the die and flip the coin.

2a) What is the probability of rolling a 1 AND flipping a heads?

2b) What is the probability of rolling a number less than 4 AND flipping tails?

2c) What is the probability of rolling a number less than 6 AND flipping heads OR tails?

2d) Suppose you’re playing a betting game where you win if you roll/flip the following combinations:

1 & heads
2 & heads
3 & heads
4 & tails
5 & tails
6 & tails
What is the probability of winning?

Question 3
3a) Suppose a process has two possible outcomes: A and B. If the probability of A (\(p(A)\)) is 0.2, what is p(B)?

3b) More generally, if a process has many possible outcomes, one of which is A, what is the probability of not A?

Question 4
The Birthday Problem is a classic problem in probability:

how many people must be in a room for there to be > 50% probability that at least two of them share a birthday?


4a) Write a function for simulating the birthday problem. The argument of the function should be the number of people in the room, and it should return the probability (from simulations, using 10,000 replicates), that two or more share a birthday. Assume there are exactly 365 days in the year and that all birthdays are equi-probable.

[Hint: if at least 2 people in a room share a birthday, the number of unique birthdays will be less than the number of people]

4b) Using this function, determine how many people must be in a room for there to be > 50% probability that at least two of them share a birthday

4c) Suppose humans colonize Mars. How many people have to be in a room on Mars for there to be a >50% probability that at least 2 of them share a Martian birthday?


## Lab6
Bhaskar Kumawat and Ivana Barnes
2025-02-14
A. Probabilities of composite events
Assume that the probability of snowing on any day in the winter is 0.3 (and independent of whether it
snowed on other days).
1. What is the probability that it does NOT snow on two consecutive days?
2. What is the probability that it does NOT snow on 10 consecutive days?
3. What is the probability that it does NOT snow on n consecutive days?
4. What is the probability that it snows on the nth day, and not on any day before that?
Let’s say you have two coins (labeled C1 and C2) and two dice (labeled D1 and D2), what is the probability
of each of these outcomes when you flip/roll all of them:
5. The sum of the two dice is 7 and both coins show heads.
6. Either:
• There is exactly one head and the sum of the dice is more than 3, or
• There are no heads and the sum of the dice is less than 6
7. C1 is heads, C2 is either heads or tails, D1 is 3, and D2 is less than 5.
B. Conditional probabilities and independence
1. If p(A) = 1
2 , p(B) = 1
11 , and events A and B are independent, what is the probability of p(A and B)?
2. Now assume that A and B are not independent, why can’t we use the same formula as in B.1 to get
p(A and B)?
3. Now, if you are given p(A|B) = 1
5 (and the values in part B.1 hold), what is p(A and B)? Are A and
B independent in this case?
4. Given, P (A) = 1
2 , P (B) = 1
11 , and p(A|B) = 1
5 , what is P (B|A)?
C. Probability of sequences
1
Let us imagine a large number of monkeys on typewriters with keys labeled A to Z (total 26). The monkeys
tap the keys completely randomly and the typewriter automatically stops working after six letters have been
typed.
1. What is the probability that a given monkey types the word “BANANA”?
2. Hence, approximately how many monkeys in a room are required to get the word BANANA typed?
Now, instead of monkeys, imagine a large number of people flipping a fair coin six times each.
1. What is the probability that a given person gets the sequence “HTTHTT”?
2. Now, assume that the coin is unfair, such that a heads appears with a probability p, and thus tails
appears with a probability q = 1 − p What is the probability that a given person gets the sequence
“HTTHTT”?
3. What is the probability that a given person gets the sequences “THTHTT” with the unfair coin?
4. With the unfair coin, out of 10,000 people, approximately how many will get the sequence “HTTHTT”?
How many will get the sequence “THTHTT”?
5. Convince yourself that each re-arrangement of “HTTHTT” will be obtained by the same number of
people as in C.4 (i.e., each rearrangement has the same probability of appearing). How many unique
re-arrangements of “HTTHTT” are there?
(Hint: think about choosing two positions for the H’s in the sequence out of six positions).
2
6. Hence, what is the total probability of getting 2 heads and 4 tails in the process (arranged in any
order)?

## Intro to Probability 2: Assignment
Due by the beginning of next Tuesday’s class
Save this Rmarkdown script as a file named “YourlastName_Assignment13.Rmd”. For each question, fill out the answer and, where requested, provide the relevant R code using “```” and the echo = TRUE argument.

When finished, Knit your script together into an html report, saved as “YourlastName_Assignment13.html” and upload the resulting file to Canvas to turn it in. It is due before our next class.



This homework assignment will test your abilities to:

think critically and creatively about probability

use simulations to build intuition

use your R skillz: function building, data visualization, etc.



Question 1
Define the following terms:

1a) random variable

1b) probability distribution function

Question 2
\(\Large {{n}\choose{k}}p^k (1-p)^{n-k}\)

2a) Using your own words, break down the equation above and describe what each part means (or is doing).

2b) Using the function of this equation that you coded up in class, calculate the probability of seeing 71 successes out of 531 trials, where the probability of success is 0.12345.

Question 3
December through March in the Northern Hemisphere will likely become a high covid prevalence season. Given the data below (taken from the Washtenaw Covid Dashboard), what is the probability that no one in the classroom has an active case of covid?

For the purposes of this calculation, assume the following:

there are 20 people in our class
each of us can be treated as a random draw from Washtenaw County
there are ~375,000 people in Washtenaw County
over the last week, Washtenaw County has averaged about 29 new cases reported per day
someone infected with covid is infectious for 10 days
only 1 in every 10 covid infections is detected.
3a) What is the analytical probability that no one in our classroom has an active covid infection?



3b) What is the probability at least one person in the room does have an active covid infection



3c) What is probability 2 people in the room are infected?



3d) Write a function for simulating this problem for gatherings of arbitrary size. The arguments of the function should be the number of people in the room and the probability that a randomly selected person in the county has an active covid infection, and it should return the probability (from simulations), that no one in the room has an active covid infection. Test it with the following class sizes: 10, 41, 100, 500.




## Probability Distribution Demonstration


Goals
1. Develop familiarity with one of a set of commonly used probability distributions
2. Establish basic skills with RShiny
3. Create a study guide to teach others about that distribution (and use their study guides to learn
about their distributions)


Overview
You will create an interactive RShiny app that introduces your assigned probability distribution to others.
In small groups in class, you will then present your distributions to each other. Your documents will serve
as a study guide to your distribution.
Organization & Timeline
1. You will be assigned a distribution from the following list:
a. (continuous): beta, exponential, gamma, lognormal, normal, uniform
b. (discrete): poisson, geometric, negative binomial, Bernoulli
2. You will then create an Rmarkdown study guide for your assigned distribution, including:
a. A brief history of the distribution
i. wikipedia can be your friend here
ii. citations unnecessary unless you make outlandish claims
b. A walkthrough of the notation, with an explanation of all parameters
c. A description of mean and variance, with intuition-(and character!)-building discussion
d. State the bounds of the distribution (if they exist), and state whether it is continuous or
discrete
e. Examples of data that are well described by the distribution (preferably biological, better
if it's an example from a field of biology that you’re interested in)
3. Shiny demo (based off the posted example)
4. Your Rmarkdown distribution study guide is due Feb 26 by 11:29am
**** NOTE: you must hand in your study guide as a .Rmd file that knits locally ***
(i.e., does not depend on any files saved locally on your computer)
