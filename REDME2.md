# LECTURE 11 – PROBABILITY AND STATISTICS: AN INTRODUCTION

**Course:** Mathematics Foundation of Machine Learning  
**Topic:** Introduction to Probability and Statistics

---

# 1. Introduction to Probability and Statistics

Probability and Statistics are two fundamental branches of mathematics that play an important role in Machine Learning, Data Science and Artificial Intelligence.

They help us understand data, analyze uncertainty, identify patterns and make predictions based on observations.

**Probability** deals with the likelihood of an event occurring.

**Statistics** deals with collecting, organizing, analyzing, interpreting and presenting data.

### Applications in Machine Learning

- Predicting future outcomes.
- Analyzing large datasets.
- Identifying patterns and trends.
- Handling uncertainty.
- Making data-driven decisions.
- Evaluating machine learning models.

# 2. Probability

## 2.1 Definition

Probability is a mathematical measure that describes how likely an event is to occur.

The probability of an event is always between 0 and 1.

$$
0\leq P(A)\leq 1
$$

Where:

- P(A) = Probability of event A.
- 0 = Impossible event.
- 1 = Certain event.

## 2.2 Basic Probability Formula

When all outcomes are equally likely:

$$
\boxed{
P(A)=\frac{\text{Number of Favorable Outcomes}}
{\text{Total Number of Possible Outcomes}}
}
$$

### Example 1: Tossing a Coin

Suppose a fair coin is tossed once.

Possible outcomes:

$$
S=\{H,T\}
$$

Where:

- H = Head
- T = Tail

Find the probability of getting a Head.

**Solution:**

Number of favorable outcomes = 1

Total possible outcomes = 2

Using the formula:

$$
P(H)=\frac{1}{2}
$$

$$
\boxed{P(H)=0.5=50\%}
$$

## 2.3 Important Terms in Probability

**Experiment:** An action or process that produces an outcome.

Example: Tossing a coin.

**Sample Space:** The set of all possible outcomes of an experiment.

Example:

$$
S=\{1,2,3,4,5,6\}
$$

For rolling a die.

**Event:** A subset of the sample space.

Example: Getting an even number.

$$
A=\{2,4,6\}
$$

**Favorable Outcomes:** Outcomes that satisfy a particular event.

## 2.4 Types of Events

**Certain Event:** An event that always occurs.

$$
P(A)=1
$$

**Impossible Event:** An event that cannot occur.

$$
P(A)=0
$$

**Complementary Event:** An event that does not occur.

$$
\boxed{P(A')=1-P(A)}
$$

**Mutually Exclusive Events:** Two events that cannot occur simultaneously.

$$
P(A\cap B)=0
$$

**Independent Events:** Two events where the occurrence of one does not affect the probability of the other.

$$
P(A\cap B)=P(A)P(B)
$$

# 3. Statistics

## 3.1 Definition

Statistics is the branch of mathematics that deals with collecting, organizing, summarizing, analyzing and interpreting data.

It helps us understand information and make decisions based on data.

## 3.2 Types of Statistics

There are two major types of statistics.

### A. Descriptive Statistics

Descriptive statistics summarizes and describes the main characteristics of a dataset.

It includes:

- Mean
- Median
- Mode
- Variance
- Standard Deviation
- Graphical Representation

### B. Inferential Statistics

Inferential statistics uses sample data to make conclusions or predictions about a larger population.

It includes:

- Hypothesis Testing
- Estimation
- Confidence Intervals
- Regression Analysis

# 4. Measures of Central Tendency

Measures of central tendency describe the center or typical value of a dataset.

The three main measures are:

1. Mean
2. Median
3. Mode

## 4.1 Mean (Arithmetic Average)

The mean is the average value of a dataset. It is calculated by dividing the sum of all observations by the total number of observations.

### Formula

$$
\boxed{
\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}
}
$$

Where:

- x̄ = Mean.
- xᵢ = Individual observations.
- n = Total number of observations.
- Σ = Summation.

### Example

Find the mean of the following dataset:

$$
X=\{10,20,30,40,50\}
$$

**Solution:**

$$
\bar{x}=\frac{10+20+30+40+50}{5}
$$

$$
=\frac{150}{5}
$$

$$
\boxed{\bar{x}=30}
$$

Therefore, the mean is 30.

## 4.2 Median

The median is the middle value of a dataset when the observations are arranged in ascending or descending order.

### Case 1: Odd Number of Observations

If n is odd:

$$
\boxed{
Median=X_{\left(\frac{n+1}{2}\right)}
}
$$

### Example

Find the median:

$$
X=\{10,20,30,40,50\}
$$

Here:

$$
n=5
$$

Median position:

$$
=\frac{5+1}{2}=3
$$

The third value is 30.

$$
\boxed{Median=30}
$$

### Case 2: Even Number of Observations

If n is even:

$$
\boxed{
Median=
\frac{
X_{\left(\frac{n}{2}\right)}
+
X_{\left(\frac{n}{2}+1\right)}
}{2}
}
$$

### Example

Find the median:

$$
X=\{10,20,30,40,50,60\}
$$

Here:

$$
n=6
$$

The two middle values are 30 and 40.

$$
Median=\frac{30+40}{2}
$$

$$
\boxed{Median=35}
$$

## 4.3 Mode

The mode is the value that occurs most frequently in a dataset.

### Example

Find the mode:

$$
X=\{10,20,20,30,40,20,50\}
$$

Here, 20 occurs three times, which is more frequent than the other values.

Therefore:

$$
\boxed{Mode=20}
$$

# 5. Measures of Dispersion

Measures of dispersion describe how spread out or scattered the observations are in a dataset.

The important measures are:

- Range
- Variance
- Standard Deviation

## 5.1 Range

Range is the difference between the maximum and minimum values in a dataset.

### Formula

$$
\boxed{
Range=X_{\max}-X_{\min}
}
$$

### Example

Given:

$$
X=\{10,20,30,40,50\}
$$

Maximum value = 50

Minimum value = 10

$$
Range=50-10
$$

$$
\boxed{Range=40}
$$

## 5.2 Variance

Variance measures how far the data values are spread from their mean.

A larger variance indicates that the data values are more spread out.

A smaller variance indicates that the values are closer to the mean.

### Population Variance Formula

$$
\boxed{
\sigma^2=
\frac{\sum_{i=1}^{N}(x_i-\mu)^2}{N}
}
$$

Where:

- σ² = Population variance.
- xᵢ = Individual observations.
- μ = Population mean.
- N = Population size.

### Sample Variance Formula

$$
\boxed{
s^2=
\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}
}
$$

Where:

- s² = Sample variance.
- x̄ = Sample mean.
- n = Sample size.

### Example: Calculate Variance

Given dataset:

$$
X=\{2,4,6,8,10\}
$$

**Step 1: Calculate Mean**

$$
\mu=\frac{2+4+6+8+10}{5}
$$

$$
\mu=\frac{30}{5}=6
$$

**Step 2: Calculate Deviations from Mean**

| x | x − μ | (x − μ)² |
|---:|---:|---:|
| 2 | -4 | 16 |
| 4 | -2 | 4 |
| 6 | 0 | 0 |
| 8 | 2 | 4 |
| 10 | 4 | 16 |
| **Total** | **0** | **40** |

**Step 3: Apply Population Variance Formula**

$$
\sigma^2=
\frac{\sum(x_i-\mu)^2}{N}
$$

$$
=\frac{40}{5}
$$

$$
\boxed{\sigma^2=8}
$$

Therefore, the population variance is 8.

## 5.3 Standard Deviation

Standard deviation is the square root of variance.

It measures how much the observations typically deviate from the mean.

### Formula

$$
\boxed{\sigma=\sqrt{\sigma^2}}
$$

### Example

From the previous example:

$$
Variance=8
$$

Therefore:

$$
\sigma=\sqrt{8}
$$

$$
\boxed{\sigma\approx2.83}
$$

**Interpretation:** The standard deviation is approximately 2.83, indicating the spread of the observations around their mean.

# 6. Outliers

## 6.1 Definition

An outlier is a data point that is significantly different from the other observations in a dataset.

It may occur because of:

- Measurement errors.
- Data entry mistakes.
- Unusual observations.
- Natural variation in data.

### Example

Consider the dataset:

$$
X=\{10,12,11,13,12,100\}
$$

Most values are between 10 and 13, but 100 is much larger than the other values.

Therefore, 100 may be considered an outlier.

## 6.2 Effect of Outliers

Outliers can significantly affect:

- Mean
- Variance
- Standard Deviation
- Machine Learning Model Performance

### Example: Effect on Mean

Without the outlier:

$$
X=\{10,12,11,13,12\}
$$

$$
Mean=\frac{10+12+11+13+12}{5}
$$

$$
=\frac{58}{5}=11.6
$$

With the outlier:

$$
X=\{10,12,11,13,12,100\}
$$

$$
Mean=\frac{158}{6}
$$

$$
\boxed{Mean\approx26.33}
$$

The outlier increases the mean significantly.

## 6.3 Detecting Outliers Using IQR

The Interquartile Range (IQR) is the difference between the third quartile and the first quartile.

$$
\boxed{IQR=Q_3-Q_1}
$$

Where:

- Q₁ = First quartile.
- Q₃ = Third quartile.

The lower and upper boundaries are:

$$
Lower=Q_1-1.5(IQR)
$$

$$
Upper=Q_3+1.5(IQR)
$$

Any observation below the lower boundary or above the upper boundary is considered a potential outlier.

# 7. Graphical Representation of Data

Graphical representation helps us understand and visualize datasets more easily.

Common graphical methods include:

1. Bar Plot
2. Scatter Plot
3. Histogram

## 7.1 Bar Plot

A bar plot is a graphical representation of categorical data using rectangular bars.

The height or length of each bar represents the frequency or value of a category.

### Example

Suppose the number of students in different departments is:

| Department | Students |
|---|---:|
| ICT | 50 |
| CSE | 40 |
| EEE | 30 |
| BBA | 20 |

A bar plot can represent the number of students in each department.

**Characteristics:**

- Used for categorical data.
- Bars are separated by spaces.
- Helps compare different categories.
- Can be vertical or horizontal.

## 7.2 Scatter Plot

A scatter plot is a graphical representation that shows the relationship between two numerical variables.

Each point represents a pair of values (x, y).

### Example

Suppose we want to understand the relationship between study hours and examination scores.

| Study Hours (X) | Marks (Y) |
|---:|---:|
| 1 | 40 |
| 2 | 50 |
| 3 | 60 |
| 4 | 70 |
| 5 | 80 |

The scatter plot can help identify whether study hours and examination marks have a positive or negative relationship.

### Types of Relationships

**Positive Correlation:** When one variable increases, the other variable also tends to increase.

**Negative Correlation:** When one variable increases, the other variable tends to decrease.

**No Correlation:** There is no clear linear relationship between the variables.

## 7.3 Histogram

A histogram is a graphical representation of the frequency distribution of numerical data.

It groups continuous numerical values into intervals called bins.

### Example

Suppose students' examination scores are grouped as follows:

| Score Range | Frequency |
|---|---:|
| 0–20 | 2 |
| 20–40 | 5 |
| 40–60 | 10 |
| 60–80 | 15 |
| 80–100 | 8 |

A histogram represents these frequency intervals using adjacent rectangular bars.

**Characteristics:**

- Used for numerical data.
- Data is grouped into bins.
- Bars usually touch each other.
- Helps understand the distribution and spread of data.

# 8. Applications of Statistics in Machine Learning

Statistics plays a major role in machine learning.

### 8.1 Data Understanding

Statistical measures help understand the basic properties of a dataset.

Examples:

- Mean
- Median
- Mode
- Variance
- Standard Deviation

### 8.2 Data Preprocessing

Statistics helps identify missing values, outliers and unusual data patterns.

### 8.3 Feature Analysis

Statistical techniques help understand relationships between different features.

### 8.4 Model Prediction

Probability helps machine learning models estimate the likelihood of different outcomes.

### 8.5 Model Evaluation

Statistical methods help evaluate model performance and reliability.

# 9. Important Mathematical Formulas

## 9.1 Probability

$$
P(A)=\frac{\text{Favorable Outcomes}}{\text{Total Outcomes}}
$$

## 9.2 Complement Rule

$$
P(A')=1-P(A)
$$

## 9.3 Mean

$$
\bar{x}=\frac{\sum x_i}{n}
$$

## 9.4 Median (Odd n)

$$
Median=X_{\left(\frac{n+1}{2}\right)}
$$

## 9.5 Median (Even n)

$$
Median=
\frac{X_{(n/2)}+X_{(n/2+1)}}{2}
$$

## 9.6 Range

$$
Range=X_{\max}-X_{\min}
$$

## 9.7 Population Variance

$$
\sigma^2=\frac{\sum(x_i-\mu)^2}{N}
$$

## 9.8 Sample Variance

$$
s^2=\frac{\sum(x_i-\bar{x})^2}{n-1}
$$

## 9.9 Standard Deviation

$$
\sigma=\sqrt{\sigma^2}
$$

## 9.10 Interquartile Range

$$
IQR=Q_3-Q_1
$$

## 9.11 Lower Outlier Boundary

$$
Lower=Q_1-1.5(IQR)
$$

## 9.12 Upper Outlier Boundary

$$
Upper=Q_3+1.5(IQR)
$$

---

# LECTURE 12 – CONDITIONAL PROBABILITY

**Course:** Mathematics Foundation of Machine Learning  
**Topic:** Conditional Probability

---

# 1. Introduction to Conditional Probability

Conditional Probability is an important concept in probability theory. It describes the probability of an event occurring when another event has already occurred.

In many real-world situations, the probability of an event depends on previously available information.

For example, suppose we want to calculate the probability that a student passes an examination given that the student attended all classes.

Here, the probability of passing depends on the condition that the student attended all classes.

Conditional probability is widely used in:

- Machine Learning
- Artificial Intelligence
- Medical Diagnosis
- Data Analysis
- Decision Making
- Bayesian Statistics

# 2. Definition of Conditional Probability

Conditional probability is the probability of an event A occurring given that another event B has already occurred.

It is represented by:

$$
P(A\mid B)
$$

Where:

- P(A | B) = Probability of event A given event B.
- A = First event.
- B = Given event or condition.

The condition B reduces the sample space to outcomes where B has occurred.

# 3. Conditional Probability Formula

The mathematical formula of conditional probability is:

$$
\boxed{
P(A\mid B)=\frac{P(A\cap B)}{P(B)}
}
$$

Where:

- P(A | B) = Conditional probability.
- P(A ∩ B) = Probability that both A and B occur.
- P(B) = Probability of event B.

**Condition:**

$$
P(B)>0
$$

This formula is used when the probability of event B is known and we want to calculate the probability of event A under that condition.

Similarly:

$$
\boxed{
P(B\mid A)=\frac{P(A\cap B)}{P(A)}
}
$$

Provided that P(A) > 0.

# 4. Understanding Conditional Probability Through a Venn Diagram

Suppose A and B are two events in a sample space.

The intersection A ∩ B represents the outcomes that belong to both events.

When calculating P(A | B), we consider only the outcomes inside B.

Therefore:

$$
P(A\mid B)=
\frac{\text{Outcomes in both A and B}}
{\text{Total outcomes in B}}
$$

This explains why the denominator is P(B), not P(A).

# 5. Solved Mathematical Examples

## Example 1: Basic Conditional Probability

**Problem:**

Suppose a class has 100 students.

- 60 students like Mathematics.
- 40 students like Statistics.
- 25 students like both Mathematics and Statistics.

Find the probability that a student likes Mathematics given that the student likes Statistics.

**Solution:**

Let:

A = Student likes Mathematics.

B = Student likes Statistics.

Given:

$$
P(A\cap B)=\frac{25}{100}
$$

$$
P(B)=\frac{40}{100}
$$

Using the conditional probability formula:

$$
P(A\mid B)=\frac{P(A\cap B)}{P(B)}
$$

Substituting the values:

$$
P(A\mid B)=
\frac{25/100}{40/100}
$$

$$
=\frac{25}{40}
$$

$$
=\boxed{0.625}
$$

Converting into percentage:

$$
0.625\times100=62.5\%
$$

**Answer:**

$$
\boxed{P(A\mid B)=62.5\%}
$$

Therefore, the probability that a student likes Mathematics given that the student likes Statistics is 62.5%.

## Example 2: Conditional Probability Using a Deck of Cards

**Problem:**

A standard deck contains 52 playing cards.

Find the probability of drawing a King given that the selected card is a face card.

**Solution:**

A standard deck contains:

- 4 Kings.
- 12 Face cards (4 Kings, 4 Queens and 4 Jacks).

Let:

A = Selecting a King.

B = Selecting a Face card.

Since all Kings are face cards:

$$
P(A\cap B)=\frac{4}{52}
$$

$$
P(B)=\frac{12}{52}
$$

Using the formula:

$$
P(A\mid B)=\frac{P(A\cap B)}{P(B)}
$$

$$
=\frac{4/52}{12/52}
$$

$$
=\frac{4}{12}
$$

$$
=\boxed{\frac{1}{3}}
$$

**Answer:**

$$
P(A\mid B)=\frac{1}{3}
$$

# 6. Multiplication Rule of Probability

The multiplication rule is derived from the conditional probability formula.

We know:

$$
P(A\mid B)=
\frac{P(A\cap B)}{P(B)}
$$

Multiplying both sides by P(B):

$$
P(A\mid B)\times P(B)=P(A\cap B)
$$

Therefore:

$$
\boxed{
P(A\cap B)=P(A\mid B)P(B)
}
$$

Similarly:

$$
\boxed{
P(A\cap B)=P(B\mid A)P(A)
}
$$

These formulas are known as the multiplication rules of probability.

## 6.1 Solved Example

**Problem:**

Suppose:

$$
P(B)=0.5
$$

And:

$$
P(A\mid B)=0.8
$$

Find P(A ∩ B).

**Solution:**

Using the multiplication rule:

$$
P(A\cap B)=P(A\mid B)P(B)
$$

Substituting:

$$
=0.8\times0.5
$$

$$
\boxed{P(A\cap B)=0.4}
$$

# 7. Addition Rule of Probability

The addition rule calculates the probability that at least one of two events occurs.

The general formula is:

$$
\boxed{
P(A\cup B)=P(A)+P(B)-P(A\cap B)
}
$$

Where:

- P(A ∪ B) = Probability that A or B or both occur.
- P(A) = Probability of event A.
- P(B) = Probability of event B.
- P(A ∩ B) = Probability of both events occurring.

## 7.1 Solved Example

**Problem:**

Suppose:

$$
P(A)=0.6
$$

$$
P(B)=0.5
$$

$$
P(A\cap B)=0.2
$$

Find P(A ∪ B).

**Solution:**

Using the addition rule:

$$
P(A\cup B)=P(A)+P(B)-P(A\cap B)
$$

Substituting:

$$
=0.6+0.5-0.2
$$

$$
\boxed{P(A\cup B)=0.9}
$$

# 8. Independent Events

Two events are independent if the occurrence of one event does not affect the probability of the other event.

For independent events:

$$
\boxed{P(A\mid B)=P(A)}
$$

Similarly:

$$
P(B\mid A)=P(B)
$$

The multiplication rule becomes:

$$
\boxed{
P(A\cap B)=P(A)P(B)
}
$$

## 8.1 Solved Example: Coin Toss and Dice Roll

**Problem:**

A coin is tossed and a die is rolled simultaneously.

Find the probability of getting a Head and a 4.

**Solution:**

Let:

A = Getting a Head.

B = Getting a 4.

Probability of getting a Head:

$$
P(A)=\frac{1}{2}
$$

Probability of getting a 4:

$$
P(B)=\frac{1}{6}
$$

Since these events are independent:

$$
P(A\cap B)=P(A)P(B)
$$

$$
=\frac{1}{2}\times\frac{1}{6}
$$

$$
\boxed{P(A\cap B)=\frac{1}{12}}
$$

# 9. Dependent Events

Two events are dependent if the occurrence of one event affects the probability of the other event.

For dependent events:

$$
P(A\mid B)\neq P(A)
$$

The multiplication rule is:

$$
\boxed{
P(A\cap B)=P(A\mid B)P(B)
}
$$

## 9.1 Solved Example: Drawing Cards Without Replacement

**Problem:**

Two cards are drawn from a standard deck of 52 cards without replacement.

Find the probability that both cards are Aces.

**Solution:**

There are 4 Aces in a deck of 52 cards.

Probability of drawing an Ace on the first draw:

$$
P(A)=\frac{4}{52}
$$

After drawing one Ace:

- Remaining cards = 51.
- Remaining Aces = 3.

Probability of drawing another Ace:

$$
P(B\mid A)=\frac{3}{51}
$$

Using the multiplication rule:

$$
P(A\cap B)=P(A)P(B\mid A)
$$

$$
=\frac{4}{52}\times\frac{3}{51}
$$

$$
=\frac{12}{2652}
$$

$$
\boxed{P(A\cap B)=\frac{1}{221}}
$$

# 10. Law of Total Probability

The Law of Total Probability is used to calculate the probability of an event by considering all possible mutually exclusive and exhaustive cases.

Suppose B₁, B₂, ..., Bₙ form a partition of the sample space.

Then:

$$
\boxed{
P(A)=\sum_{i=1}^{n}P(A\mid B_i)P(B_i)
}
$$

For two events B and B':

$$
\boxed{
P(A)=P(A\mid B)P(B)
+
P(A\mid B')P(B')
}
$$

Where:

- B' = Complement of B.
- P(B) + P(B') = 1.

## 10.1 Solved Example

**Problem:**

A factory has two machines, A and B.

- Machine A produces 60% of the products.
- Machine B produces 40% of the products.
- Machine A produces 2% defective products.
- Machine B produces 5% defective products.

Find the probability that a randomly selected product is defective.

**Solution:**

Let:

D = Selecting a defective product.

A = Product manufactured by Machine A.

B = Product manufactured by Machine B.

Given:

$$
P(A)=0.60
$$

$$
P(B)=0.40
$$

$$
P(D\mid A)=0.02
$$

$$
P(D\mid B)=0.05
$$

Using the Law of Total Probability:

$$
P(D)=P(D\mid A)P(A)
+
P(D\mid B)P(B)
$$

Substituting:

$$
=(0.02\times0.60)
+(0.05\times0.40)
$$

$$
=0.012+0.020
$$

$$
\boxed{P(D)=0.032}
$$

Converting into percentage:

$$
0.032\times100=3.2\%
$$

**Answer:** The probability of selecting a defective product is 3.2%.

# 11. Important Properties of Conditional Probability

**Property 1:**

$$
0\leq P(A\mid B)\leq1
$$

**Property 2:**

$$
P(B)>0
$$

**Property 3:**

$$
P(A\mid B)=
\frac{P(A\cap B)}{P(B)}
$$

**Property 4:**

$$
P(A\cap B)=P(A\mid B)P(B)
$$

**Property 5:**

For independent events:

$$
P(A\mid B)=P(A)
$$

**Property 6:**

For any event A:

$$
P(A\mid A)=1
$$

Provided that P(A) > 0.

# 12. Important Mathematical Formulas

## 12.1 Conditional Probability

$$
P(A\mid B)=
\frac{P(A\cap B)}{P(B)}
$$

## 12.2 Reverse Conditional Probability

$$
P(B\mid A)=
\frac{P(A\cap B)}{P(A)}
$$

## 12.3 Multiplication Rule

$$
P(A\cap B)=P(A\mid B)P(B)
$$

## 12.4 Addition Rule

$$
P(A\cup B)=P(A)+P(B)-P(A\cap B)
$$

## 12.5 Independent Events

$$
P(A\cap B)=P(A)P(B)
$$

## 12.6 Independent Conditional Probability

$$
P(A\mid B)=P(A)
$$

## 12.7 Law of Total Probability

$$
P(A)=\sum_{i=1}^{n}P(A\mid B_i)P(B_i)
$$

## 12.8 Complement Rule

$$
P(A')=1-P(A)
$$

---

# Lecture 13: Bayes’ Theorem

## 1. Introduction

Bayes’ Theorem is an important concept in probability and statistics. It is used to calculate the probability of an event based on previously known information or evidence.

It helps us update the probability of an event when new information becomes available. Bayes’ Theorem is widely used in Machine Learning, medical diagnosis, spam detection, and decision-making.

## 2. Definition of Bayes’ Theorem

Bayes’ Theorem describes the relationship between conditional probabilities. It calculates the probability of event A occurring given that event B has already occurred.

The formula is:

$$
P(A|B)=\frac{P(B|A)\times P(A)}{P(B)}
$$

Where,

- \(P(A|B)\) = Posterior probability: Probability of A given B.
- \(P(B|A)\) = Likelihood: Probability of B given A.
- \(P(A)\) = Prior probability: Initial probability of A.
- \(P(B)\) = Evidence: Total probability of B.

## 3. Derivation of Bayes’ Theorem

From the conditional probability formula,

$$
P(A|B)=\frac{P(A\cap B)}{P(B)}
$$

Similarly,

$$
P(B|A)=\frac{P(A\cap B)}{P(A)}
$$

Rearranging the second equation,

$$
P(A\cap B)=P(B|A)\times P(A)
$$

Substituting this value into the first equation,

$$
P(A|B)=\frac{P(B|A)\times P(A)}{P(B)}
$$

Therefore, the Bayes’ Theorem is:

$$
\boxed{P(A|B)=\frac{P(B|A)P(A)}{P(B)}}
$$

## 4. Bayes’ Theorem Using Two Events

Suppose A and B are two events, and \(P(B)>0\).

Bayes’ Theorem determines the probability of A when B is known to have occurred.

$$
P(A|B)=\frac{P(B|A)P(A)}{P(B)}
$$

If the events A and its complement \(\bar A\) cover all possible cases, then:

$$
P(B)=P(B|A)P(A)+P(B|\bar A)P(\bar A)
$$

Therefore,

$$
P(A|B)=
\frac{P(B|A)P(A)}
{P(B|A)P(A)+P(B|\bar A)P(\bar A)}
$$

## 5. Solved Numerical Example 1

**Problem:**

A disease affects 1% of a population. A medical test correctly identifies a person with the disease 90% of the time. The test also gives a positive result for 5% of healthy people.

If a person tests positive, find the probability that the person actually has the disease.

**Solution:**

Let,

- A = Person has the disease.
- \(\bar A\) = Person does not have the disease.
- B = Test result is positive.

Given,

$$
P(A)=0.01
$$

$$
P(\bar A)=0.99
$$

$$
P(B|A)=0.90
$$

$$
P(B|\bar A)=0.05
$$

Using Bayes’ Theorem,

$$
P(A|B)=
\frac{P(B|A)P(A)}
{P(B|A)P(A)+P(B|\bar A)P(\bar A)}
$$

Substituting the values,

$$
P(A|B)=
\frac{0.90\times0.01}
{(0.90\times0.01)+(0.05\times0.99)}
$$

$$
=\frac{0.009}{0.009+0.0495}
$$

$$
=\frac{0.009}{0.0585}
$$

$$
=0.1538
$$

Therefore,

$$
\boxed{P(A|B)=15.38\%}
$$

**Answer:** The probability that the person actually has the disease is approximately 15.38%.

## 6. Solved Numerical Example 2

**Problem:**

A factory has two machines, A and B. Machine A produces 60% of the total products, while machine B produces 40%. Machine A produces 2% defective products, and machine B produces 5% defective products.

If a randomly selected product is defective, find the probability that it was produced by machine B.

**Solution:**

Let,

- A = Product produced by machine A.
- B = Product produced by machine B.
- D = Product is defective.

Given,

$$
P(A)=0.60
$$

$$
P(B)=0.40
$$

$$
P(D|A)=0.02
$$

$$
P(D|B)=0.05
$$

We need to find:

$$
P(B|D)
$$

Using Bayes’ Theorem,

$$
P(B|D)=\frac{P(D|B)P(B)}{P(D)}
$$

First, calculate the total probability of a defective product:

$$
P(D)=P(D|A)P(A)+P(D|B)P(B)
$$

$$
=(0.02\times0.60)+(0.05\times0.40)
$$

$$
=0.012+0.020
$$

$$
=0.032
$$

Now,

$$
P(B|D)=\frac{0.05\times0.40}{0.032}
$$

$$
=\frac{0.020}{0.032}
$$

$$
=0.625
$$

Therefore,

$$
\boxed{P(B|D)=62.5\%}
$$

**Answer:** The probability that the defective product was produced by machine B is 62.5%.

## 7. Applications of Bayes’ Theorem

Bayes’ Theorem is used in many practical fields:

1. **Medical Diagnosis:** Finding the probability of a disease based on test results.
2. **Spam Detection:** Determining whether an email is spam based on its words and features.
3. **Machine Learning:** Used in Naive Bayes classification algorithms.
4. **Weather Forecasting:** Updating the probability of weather conditions using new observations.
5. **Decision Making:** Updating beliefs and probabilities when new evidence becomes available.

## 8. Important Formulas

**Bayes’ Theorem:**

$$
P(A|B)=\frac{P(B|A)P(A)}{P(B)}
$$

**Conditional Probability:**

$$
P(A|B)=\frac{P(A\cap B)}{P(B)}
$$

**Law of Total Probability:**

$$
P(B)=P(B|A)P(A)+P(B|\bar A)P(\bar A)
$$

**Complement Rule:**

$$
P(\bar A)=1-P(A)
$$

**Joint Probability:**

$$
P(A\cap B)=P(B|A)P(A)
$$

**Remember:** Bayes’ Theorem is used to update the prior probability of an event using new evidence and calculate its posterior probability.

---

**END OF LECTURE 13**
