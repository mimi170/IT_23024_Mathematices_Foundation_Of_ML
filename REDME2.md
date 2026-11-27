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
# Lecture 14: Probability Distributions

## 1. Introduction

A Probability Distribution describes how the probabilities of different possible outcomes of a random variable are distributed.

It tells us how likely each value of a random variable is to occur.

Probability distributions are important in statistics, probability theory, and Machine Learning because they help us understand uncertainty and analyze data.

## 2. Random Variable

A random variable is a variable whose value depends on the outcome of a random experiment.

It is usually represented by a capital letter such as \(X\).

**Example:**

When a coin is tossed, the possible outcomes are:

$$
S=\{H,T\}
$$

Let,

$$
X=
\begin{cases}
1 & \text{if Head occurs}\\
0 & \text{if Tail occurs}
\end{cases}
$$

Here, \(X\) is a random variable because its value depends on the outcome of the coin toss.

## 3. Types of Random Variables

There are two main types of random variables.

### 3.1 Discrete Random Variable

A discrete random variable takes countable values.

**Examples:**

- Number of students in a classroom.
- Number of heads in three coin tosses.
- Number of defective products in a batch.
- Number of customers visiting a shop.

For example, when a coin is tossed three times, the number of heads can be:

$$
X=\{0,1,2,3\}
$$

### 3.2 Continuous Random Variable

A continuous random variable can take any value within a given interval.

**Examples:**

- Height of a person.
- Weight of a student.
- Temperature of a city.
- Time required to complete a task.

For example, a person's height may be 160.5 cm, 160.55 cm, or 160.555 cm.

## 4. Probability Distribution

A probability distribution is a mathematical function that describes the possible values of a random variable and their corresponding probabilities.

For a discrete random variable, the probability distribution must satisfy two conditions:

**Condition 1:**

Every probability must be between 0 and 1.

$$
0\leq P(X=x)\leq 1
$$

**Condition 2:**

The sum of all probabilities must be equal to 1.

$$
\sum_x P(X=x)=1
$$

## 5. Probability Mass Function (PMF)

A Probability Mass Function (PMF) gives the probability that a discrete random variable takes a particular value.

It is represented by:

$$
P(X=x)
$$

**Example:**

A fair coin is tossed twice. Find the probability distribution of the number of heads.

**Solution:**

Possible outcomes:

$$
S=\{HH,HT,TH,TT\}
$$

Let \(X\) be the number of heads.

| Outcome | Number of Heads (X) |
|---|---:|
| HH | 2 |
| HT | 1 |
| TH | 1 |
| TT | 0 |

The probability distribution is:

| X | P(X) |
|---:|---:|
| 0 | 1/4 |
| 1 | 2/4 |
| 2 | 1/4 |

Checking the total probability:

$$
\sum P(X)=\frac14+\frac24+\frac14
$$

$$
=1
$$

Therefore, the probability distribution is valid.

## 6. Probability Density Function (PDF)

A Probability Density Function (PDF) describes the probability distribution of a continuous random variable.

It is represented by:

$$
f(x)
$$

For a continuous random variable, the probability of a particular exact value is zero.

$$
P(X=a)=0
$$

The probability that a random variable lies between two values \(a\) and \(b\) is calculated using integration.

$$
P(a\leq X\leq b)=\int_a^b f(x)\,dx
$$

A valid PDF must satisfy two conditions:

**Condition 1:**

$$
f(x)\geq 0
$$

**Condition 2:**

The total area under the PDF curve must be equal to 1.

$$
\int_{-\infty}^{\infty}f(x)\,dx=1
$$

## 7. Cumulative Distribution Function (CDF)

A Cumulative Distribution Function (CDF) gives the probability that a random variable \(X\) takes a value less than or equal to a particular value \(x\).

It is represented by:

$$
F(x)=P(X\leq x)
$$

For a discrete random variable:

$$
F(x)=\sum_{t\leq x}P(X=t)
$$

For a continuous random variable:

$$
F(x)=\int_{-\infty}^{x}f(t)\,dt
$$

**Example:**

Suppose a random variable has the following probability distribution:

| X | P(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.3 |
| 3 | 0.5 |

Find the CDF values.

**Solution:**

For \(X=1\):

$$
F(1)=P(X\leq1)=0.2
$$

For \(X=2\):

$$
F(2)=P(X\leq2)
$$

$$
=0.2+0.3=0.5
$$

For \(X=3\):

$$
F(3)=P(X\leq3)
$$

$$
=0.2+0.3+0.5=1
$$

Therefore:

| X | F(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.5 |
| 3 | 1.0 |

## 8. Expected Value (Mean)

The expected value is the average or long-run mean value of a random variable.

It is represented by:

$$
E(X)
$$

For a discrete random variable:

$$
E(X)=\sum_x xP(X=x)
$$

Where:

- \(x\) = Possible value of the random variable.
- \(P(X=x)\) = Probability of that value.

**Example:**

Suppose the probability distribution is:

| X | P(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.3 |
| 3 | 0.5 |

Find the expected value.

**Solution:**

$$
E(X)=\sum_x xP(X=x)
$$

$$
=(1\times0.2)+(2\times0.3)+(3\times0.5)
$$

$$
=0.2+0.6+1.5
$$

$$
\boxed{E(X)=2.3}
$$

Therefore, the expected value is 2.3.

## 9. Variance of a Random Variable

Variance measures how far the values of a random variable are spread around its mean.

It is represented by:

$$
Var(X)
$$

The formula is:

$$
Var(X)=E[(X-\mu)^2]
$$

Another commonly used formula is:

$$
Var(X)=E(X^2)-[E(X)]^2
$$

Where:

- \(E(X^2)\) = Expected value of the square of X.
- \(E(X)\) = Mean or expected value.
- \(\mu\) = Population mean.

**Example:**

Using the previous probability distribution:

| X | P(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.3 |
| 3 | 0.5 |

We already calculated:

$$
E(X)=2.3
$$

First, calculate \(E(X^2)\).

$$
E(X^2)=\sum_x x^2P(X=x)
$$

$$
=(1^2\times0.2)+(2^2\times0.3)+(3^2\times0.5)
$$

$$
=0.2+1.2+4.5
$$

$$
=5.9
$$

Now, calculate variance.

$$
Var(X)=E(X^2)-[E(X)]^2
$$

$$
=5.9-(2.3)^2
$$

$$
=5.9-5.29
$$

$$
\boxed{Var(X)=0.61}
$$

## 10. Standard Deviation

Standard deviation measures the spread of values around the mean. It is the square root of variance.

The formula is:

$$
\sigma=\sqrt{Var(X)}
$$

Using the previous example:

$$
\sigma=\sqrt{0.61}
$$

$$
\boxed{\sigma\approx0.781}
$$

## 11. Important Formulas

**Probability Mass Function:**

$$
P(X=x)
$$

**Probability Density Function:**

$$
P(a\leq X\leq b)=\int_a^b f(x)\,dx
$$

**Cumulative Distribution Function:**

$$
F(x)=P(X\leq x)
$$

**Expected Value:**

$$
E(X)=\sum_x xP(X=x)
$$

**Variance:**

$$
Var(X)=E(X^2)-[E(X)]^2
$$

**Standard Deviation:**

$$
\sigma=\sqrt{Var(X)}
$$
# Lecture 14: Probability Distributions

## 1. Introduction

A Probability Distribution describes how the probabilities of different possible outcomes of a random variable are distributed.

It tells us how likely each value of a random variable is to occur.

Probability distributions are important in statistics, probability theory, and Machine Learning because they help us understand uncertainty and analyze data.

## 2. Random Variable

A random variable is a variable whose value depends on the outcome of a random experiment.

It is usually represented by a capital letter such as \(X\).

**Example:**

When a coin is tossed, the possible outcomes are:

$$
S=\{H,T\}
$$

Let,

$$
X=
\begin{cases}
1 & \text{if Head occurs}\\
0 & \text{if Tail occurs}
\end{cases}
$$

Here, \(X\) is a random variable because its value depends on the outcome of the coin toss.

## 3. Types of Random Variables

There are two main types of random variables.

### 3.1 Discrete Random Variable

A discrete random variable takes countable values.

**Examples:**

- Number of students in a classroom.
- Number of heads in three coin tosses.
- Number of defective products in a batch.
- Number of customers visiting a shop.

For example, when a coin is tossed three times, the number of heads can be:

$$
X=\{0,1,2,3\}
$$

### 3.2 Continuous Random Variable

A continuous random variable can take any value within a given interval.

**Examples:**

- Height of a person.
- Weight of a student.
- Temperature of a city.
- Time required to complete a task.

For example, a person's height may be 160.5 cm, 160.55 cm, or 160.555 cm.

## 4. Probability Distribution

A probability distribution is a mathematical function that describes the possible values of a random variable and their corresponding probabilities.

For a discrete random variable, the probability distribution must satisfy two conditions:

**Condition 1:**

Every probability must be between 0 and 1.

$$
0\leq P(X=x)\leq 1
$$

**Condition 2:**

The sum of all probabilities must be equal to 1.

$$
\sum_x P(X=x)=1
$$

## 5. Probability Mass Function (PMF)

A Probability Mass Function (PMF) gives the probability that a discrete random variable takes a particular value.

It is represented by:

$$
P(X=x)
$$

**Example:**

A fair coin is tossed twice. Find the probability distribution of the number of heads.

**Solution:**

Possible outcomes:

$$
S=\{HH,HT,TH,TT\}
$$

Let \(X\) be the number of heads.

| Outcome | Number of Heads (X) |
|---|---:|
| HH | 2 |
| HT | 1 |
| TH | 1 |
| TT | 0 |

The probability distribution is:

| X | P(X) |
|---:|---:|
| 0 | 1/4 |
| 1 | 2/4 |
| 2 | 1/4 |

Checking the total probability:

$$
\sum P(X)=\frac14+\frac24+\frac14
$$

$$
=1
$$

Therefore, the probability distribution is valid.

## 6. Probability Density Function (PDF)

A Probability Density Function (PDF) describes the probability distribution of a continuous random variable.

It is represented by:

$$
f(x)
$$

For a continuous random variable, the probability of a particular exact value is zero.

$$
P(X=a)=0
$$

The probability that a random variable lies between two values \(a\) and \(b\) is calculated using integration.

$$
P(a\leq X\leq b)=\int_a^b f(x)\,dx
$$

A valid PDF must satisfy two conditions:

**Condition 1:**

$$
f(x)\geq 0
$$

**Condition 2:**

The total area under the PDF curve must be equal to 1.

$$
\int_{-\infty}^{\infty}f(x)\,dx=1
$$

## 7. Cumulative Distribution Function (CDF)

A Cumulative Distribution Function (CDF) gives the probability that a random variable \(X\) takes a value less than or equal to a particular value \(x\).

It is represented by:

$$
F(x)=P(X\leq x)
$$

For a discrete random variable:

$$
F(x)=\sum_{t\leq x}P(X=t)
$$

For a continuous random variable:

$$
F(x)=\int_{-\infty}^{x}f(t)\,dt
$$

**Example:**

Suppose a random variable has the following probability distribution:

| X | P(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.3 |
| 3 | 0.5 |

Find the CDF values.

**Solution:**

For \(X=1\):

$$
F(1)=P(X\leq1)=0.2
$$

For \(X=2\):

$$
F(2)=P(X\leq2)
$$

$$
=0.2+0.3=0.5
$$

For \(X=3\):

$$
F(3)=P(X\leq3)
$$

$$
=0.2+0.3+0.5=1
$$

Therefore:

| X | F(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.5 |
| 3 | 1.0 |

## 8. Expected Value (Mean)

The expected value is the average or long-run mean value of a random variable.

It is represented by:

$$
E(X)
$$

For a discrete random variable:

$$
E(X)=\sum_x xP(X=x)
$$

Where:

- \(x\) = Possible value of the random variable.
- \(P(X=x)\) = Probability of that value.

**Example:**

Suppose the probability distribution is:

| X | P(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.3 |
| 3 | 0.5 |

Find the expected value.

**Solution:**

$$
E(X)=\sum_x xP(X=x)
$$

$$
=(1\times0.2)+(2\times0.3)+(3\times0.5)
$$

$$
=0.2+0.6+1.5
$$

$$
\boxed{E(X)=2.3}
$$

Therefore, the expected value is 2.3.

## 9. Variance of a Random Variable

Variance measures how far the values of a random variable are spread around its mean.

It is represented by:

$$
Var(X)
$$

The formula is:

$$
Var(X)=E[(X-\mu)^2]
$$

Another commonly used formula is:

$$
Var(X)=E(X^2)-[E(X)]^2
$$

Where:

- \(E(X^2)\) = Expected value of the square of X.
- \(E(X)\) = Mean or expected value.
- \(\mu\) = Population mean.

**Example:**

Using the previous probability distribution:

| X | P(X) |
|---:|---:|
| 1 | 0.2 |
| 2 | 0.3 |
| 3 | 0.5 |

We already calculated:

$$
E(X)=2.3
$$

First, calculate \(E(X^2)\).

$$
E(X^2)=\sum_x x^2P(X=x)
$$

$$
=(1^2\times0.2)+(2^2\times0.3)+(3^2\times0.5)
$$

$$
=0.2+1.2+4.5
$$

$$
=5.9
$$

Now, calculate variance.

$$
Var(X)=E(X^2)-[E(X)]^2
$$

$$
=5.9-(2.3)^2
$$

$$
=5.9-5.29
$$

$$
\boxed{Var(X)=0.61}
$$

## 10. Standard Deviation

Standard deviation measures the spread of values around the mean. It is the square root of variance.

The formula is:

$$
\sigma=\sqrt{Var(X)}
$$

Using the previous example:

$$
\sigma=\sqrt{0.61}
$$

$$
\boxed{\sigma\approx0.781}
$$

## 11. Important Formulas

**Probability Mass Function:**

$$
P(X=x)
$$

**Probability Density Function:**

$$
P(a\leq X\leq b)=\int_a^b f(x)\,dx
$$

**Cumulative Distribution Function:**

$$
F(x)=P(X\leq x)
$$

**Expected Value:**

$$
E(X)=\sum_x xP(X=x)
$$

**Variance:**

$$
Var(X)=E(X^2)-[E(X)]^2
$$

**Standard Deviation:**

$$
\sigma=\sqrt{Var(X)}
$$

---

# Lecture 15: Hypothesis Testing

## 1. Introduction

Hypothesis Testing is a statistical method used to make decisions or draw conclusions about a population based on sample data.

It helps us determine whether there is enough statistical evidence to support a particular assumption or claim.

In Machine Learning and Statistics, hypothesis testing is used to analyze data, test assumptions, and evaluate the significance of results.

## 2. What is a Hypothesis?

A hypothesis is a statement or assumption about a population parameter that can be tested using statistical methods.

**Example:**

Suppose a university claims that the average study time of its students is 5 hours per day.

We can collect sample data and test whether this claim is supported by the evidence.

## 3. Types of Hypothesis

There are two main types of hypotheses.

### 3.1 Null Hypothesis (H₀)

The Null Hypothesis represents the initial assumption that there is no significant effect, difference, or relationship between variables.

It is denoted by:

$$
H_0
$$

**Example:**

$$
H_0:\mu=5
$$

Here, \(\mu\) represents the population mean.

### 3.2 Alternative Hypothesis (H₁)

The Alternative Hypothesis represents the statement that contradicts the null hypothesis.

It indicates that there is a significant effect, difference, or relationship.

It is denoted by:

$$
H_1
$$

For the previous example:

$$
H_1:\mu\neq5
$$

This means the average study time is not equal to 5 hours.

## 4. Types of Alternative Hypothesis

### 4.1 Two-Tailed Test

A two-tailed test is used when we want to determine whether a population parameter is either greater than or less than a specified value.

Example:

$$
H_0:\mu=50
$$

$$
H_1:\mu\neq50
$$

### 4.2 Right-Tailed Test

A right-tailed test is used when we want to determine whether the population parameter is greater than a specified value.

Example:

$$
H_0:\mu=50
$$

$$
H_1:\mu>50
$$

### 4.3 Left-Tailed Test

A left-tailed test is used when we want to determine whether the population parameter is less than a specified value.

Example:

$$
H_0:\mu=50
$$

$$
H_1:\mu<50
$$

## 5. Significance Level (α)

The significance level is the probability of rejecting the null hypothesis when it is actually true.

It is denoted by:

$$
\alpha
$$

Common significance levels are:

- 0.10 or 10%
- 0.05 or 5%
- 0.01 or 1%

For example, if:

$$
\alpha=0.05
$$

It means we accept a 5% risk of making a Type I error.

## 6. P-Value

The P-value is the probability of obtaining a result as extreme as, or more extreme than, the observed result, assuming that the null hypothesis is true.

It helps us decide whether the sample evidence is statistically significant.

**Decision Rule:**

- If P-value ≤ α, reject the null hypothesis.
- If P-value > α, fail to reject the null hypothesis.

**Example:**

Suppose:

$$
P\text{-value}=0.03
$$

And,

$$
\alpha=0.05
$$

Since,

$$
0.03<0.05
$$

We reject the null hypothesis.

## 7. Type I and Type II Errors

### 7.1 Type I Error

A Type I error occurs when we reject the null hypothesis even though it is actually true.

It is represented by:

$$
\alpha
$$

**Example:** A medical test concludes that a healthy person has a disease.

### 7.2 Type II Error

A Type II error occurs when we fail to reject the null hypothesis even though it is actually false.

It is represented by:

$$
\beta
$$

**Example:** A medical test concludes that a person does not have a disease when the person actually has it.

## 8. Test Statistic

A test statistic is a numerical value calculated from sample data. It is used to determine whether the null hypothesis should be rejected.

The general Z-test formula for a population mean, when the population standard deviation is known, is:

$$
Z=\frac{\bar{x}-\mu}{\sigma/\sqrt{n}}
$$

Where:

- \(\bar{x}\) = Sample mean.
- \(\mu\) = Population mean under the null hypothesis.
- \(\sigma\) = Population standard deviation.
- \(n\) = Sample size.

## 9. Z-Test

A Z-test is a statistical test used to determine whether there is a significant difference between a sample statistic and a population parameter.

It is commonly used when the population standard deviation is known and the sampling distribution is normal or the sample size is sufficiently large.

**Formula:**

$$
Z=\frac{\bar{x}-\mu}{\sigma/\sqrt{n}}
$$

### Solved Numerical Example

**Problem:**

A company claims that the average weight of its product is 50 kg. A sample of 36 products has an average weight of 52 kg. The population standard deviation is 6 kg.

Test the company's claim at a 5% significance level using a two-tailed Z-test.

**Solution:**

Given:

$$
\mu=50,\quad \bar{x}=52
$$

$$
\sigma=6,\quad n=36
$$

$$
\alpha=0.05
$$

**Step 1: Formulate the Hypotheses**

$$
H_0:\mu=50
$$

$$
H_1:\mu\neq50
$$

**Step 2: Calculate the Test Statistic**

$$
Z=\frac{\bar{x}-\mu}{\sigma/\sqrt{n}}
$$

$$
Z=\frac{52-50}{6/\sqrt{36}}
$$

$$
=\frac{2}{6/6}
$$

$$
=\frac{2}{1}
$$

$$
\boxed{Z=2}
$$

**Step 3: Determine the Critical Value**

For a two-tailed test at a 5% significance level:

$$
Z_{\text{critical}}=\pm1.96
$$

**Step 4: Make the Decision**

Since,

$$
|Z|=2>1.96
$$

We reject the null hypothesis.

**Answer:** There is sufficient statistical evidence at the 5% significance level to conclude that the average product weight is different from 50 kg.

## 10. T-Test

A T-test is a statistical test used to determine whether there is a significant difference between means.

It is generally used when the population standard deviation is unknown, especially for small samples when the data are approximately normally distributed.

For a one-sample T-test, the formula is:

$$
t=\frac{\bar{x}-\mu}{s/\sqrt{n}}
$$

Where:

- \(\bar{x}\) = Sample mean.
- \(\mu\) = Hypothesized population mean.
- \(s\) = Sample standard deviation.
- \(n\) = Sample size.

The degrees of freedom are:

$$
df=n-1
$$

## 11. Confidence Interval

A confidence interval is a range of values used to estimate an unknown population parameter based on sample data.

For a population mean with known population standard deviation, the confidence interval is:

$$
\bar{x}\pm Z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
$$

Where:

- \(\bar{x}\) = Sample mean.
- \(Z_{\alpha/2}\) = Critical Z-value.
- \(\sigma\) = Population standard deviation.
- \(n\) = Sample size.

For example, a 95% confidence interval uses:

$$
Z_{\alpha/2}=1.96
$$

## 12. Steps of Hypothesis Testing

1. State the null hypothesis (\(H_0\)).
2. State the alternative hypothesis (\(H_1\)).
3. Select the significance level (\(\alpha\)).
4. Choose the appropriate statistical test.
5. Calculate the test statistic using sample data.
6. Determine the P-value or critical value.
7. Reject or fail to reject the null hypothesis.
8. Interpret the result in the context of the problem.

## 13. Applications of Hypothesis Testing

1. **Machine Learning:** Evaluating whether a model improvement is statistically significant.
2. **Medical Research:** Testing the effectiveness of medicines and treatments.
3. **Business:** Evaluating changes in sales, profit, and customer behavior.
4. **Education:** Testing whether a new teaching method improves student performance.
5. **Scientific Research:** Testing assumptions and validating research findings.

## 14. Important Formulas

**Z-Test:**

$$
Z=\frac{\bar{x}-\mu}{\sigma/\sqrt{n}}
$$

**T-Test:**

$$
t=\frac{\bar{x}-\mu}{s/\sqrt{n}}
$$

**Degrees of Freedom:**

$$
df=n-1
$$

**Confidence Interval:**

$$
\bar{x}\pm Z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
$$

**Decision Rule:**

$$
P\text{-value}\leq\alpha
\Rightarrow \text{Reject }H_0
$$

$$
P\text{-value}>\alpha
\Rightarrow \text{Fail to reject }H_0
$$

# Lecture 16: Naive Bayes Classification and Model Evaluation

## 1. Introduction

Naive Bayes is a supervised Machine Learning algorithm based on Bayes' Theorem. It is mainly used for classification problems.

It predicts the class of a given data point by calculating the probability of each possible class.

Model Evaluation is the process of measuring how well a Machine Learning model performs on a dataset.

Confusion Matrix, Accuracy, Precision, Recall, and F1-Score are commonly used evaluation techniques for classification models.

## 2. Naive Bayes Classifier

Naive Bayes is a probabilistic classification algorithm based on Bayes' Theorem.

It is called "Naive" because it assumes that all features are conditionally independent given the class label.

The general Bayes' Theorem is:

$$
P(A|B)=\frac{P(B|A)P(A)}{P(B)}
$$

For classification, the formula becomes:

$$
P(C|X)=\frac{P(X|C)P(C)}{P(X)}
$$

Where:

- \(P(C|X)\) = Posterior probability of class C given features X.
- \(P(X|C)\) = Likelihood of features X given class C.
- \(P(C)\) = Prior probability of class C.
- \(P(X)\) = Evidence or probability of features X.

The predicted class is:

$$
C_{\text{predicted}}=\arg\max_C P(C|X)
$$

Since \(P(X)\) is the same for all classes, we can write:

$$
C_{\text{predicted}}=\arg\max_C P(X|C)P(C)
$$

## 3. Naive Bayes Assumption

The Naive Bayes classifier assumes that all features are conditionally independent of each other given the class.

For example, suppose we want to classify an email as Spam or Not Spam using two features:

- Contains the word "Free".
- Contains the word "Offer".

Under the Naive Bayes assumption:

$$
P(X_1,X_2|C)=P(X_1|C)P(X_2|C)
$$

For multiple features:

$$
P(X|C)=\prod_{i=1}^{n}P(X_i|C)
$$

Where:

- \(X_i\) = Individual feature.
- \(C\) = Class label.
- \(n\) = Total number of features.

## 4. Types of Naive Bayes Classifier

There are three commonly used types of Naive Bayes classifiers.

### 4.1 Gaussian Naive Bayes

Gaussian Naive Bayes is used when the features are continuous numerical values.

It assumes that the values of each feature follow a Gaussian (Normal) distribution within each class.

The Gaussian probability density function is:

$$
P(x|C)=\frac{1}{\sqrt{2\pi\sigma^2}}
e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

Where:

- \(x\) = Observed feature value.
- \(\mu\) = Mean of the feature for a particular class.
- \(\sigma^2\) = Variance of the feature for a particular class.
- \(\pi\) = Mathematical constant.

**Example:**

Predicting whether a person belongs to a particular category based on continuous features such as height, weight, or temperature.

### 4.2 Multinomial Naive Bayes

Multinomial Naive Bayes is commonly used for text classification.

It works with discrete feature counts, such as the number of times a word appears in a document.

The probability of a feature is:

$$
P(X_i|C)=
\frac{\text{Count}(X_i,C)+\alpha}
{\text{Total feature count in C}+\alpha V}
$$

Where:

- \(\text{Count}(X_i,C)\) = Count of feature \(X_i\) in class C.
- \(\alpha\) = Smoothing parameter.
- \(V\) = Number of unique features in the vocabulary.

**Example:**

Classifying emails as Spam or Not Spam based on word frequencies.

### 4.3 Bernoulli Naive Bayes

Bernoulli Naive Bayes is used when features are binary.

Each feature can have only two possible values:

$$
X_i\in\{0,1\}
$$

Where:

- 1 = Feature is present.
- 0 = Feature is absent.

**Example:**

Classifying an email based on whether certain words are present or absent.

## 5. Laplace Smoothing

Laplace Smoothing is used in Naive Bayes to avoid zero probabilities.

Sometimes a particular feature does not appear in the training data for a class. Without smoothing, its probability becomes zero.

Since Naive Bayes multiplies probabilities, a single zero probability can make the entire class probability zero.

The Laplace smoothing formula is:

$$
P(X_i|C)=
\frac{\text{Count}(X_i,C)+1}
{\text{Total count in C}+V}
$$

Where:

- \(X_i\) = Feature.
- \(C\) = Class.
- \(V\) = Number of unique features.

The value 1 is added to each feature count to prevent zero probabilities.

## 6. Solved Example of Naive Bayes Classification

**Problem:**

Suppose an email contains the word "Free". We want to predict whether the email is Spam or Not Spam.

Given:

$$
P(Spam)=0.4
$$

$$
P(Not\ Spam)=0.6
$$

$$
P(Free|Spam)=0.8
$$

$$
P(Free|Not\ Spam)=0.1
$$

Find the probability that the email is Spam given that it contains the word "Free".

**Solution:**

Using Bayes' Theorem:

$$
P(Spam|Free)=
\frac{P(Free|Spam)P(Spam)}
{P(Free)}
$$

First, calculate \(P(Free)\):

$$
P(Free)=P(Free|Spam)P(Spam)
$$

$$
+P(Free|Not\ Spam)P(Not\ Spam)
$$

Substituting the values:

$$
=(0.8\times0.4)+(0.1\times0.6)
$$

$$
=0.32+0.06
$$

$$
=0.38
$$

Now calculate:

$$
P(Spam|Free)=\frac{0.8\times0.4}{0.38}
$$

$$
=\frac{0.32}{0.38}
$$

$$
=0.8421
$$

Therefore:

$$
\boxed{P(Spam|Free)=84.21\%}
$$

**Answer:** The probability that the email is Spam is approximately 84.21%.

## 7. Machine Learning Model Evaluation

Model Evaluation is the process of measuring the performance of a Machine Learning model.

It helps us understand how accurately a model predicts the output for unseen data.

For classification problems, common evaluation metrics include:

1. Confusion Matrix.
2. Accuracy.
3. Precision.
4. Recall.
5. F1-Score.

## 8. Confusion Matrix

A Confusion Matrix is a table used to evaluate the performance of a classification model.

It compares the actual class labels with the predicted class labels.

For binary classification, the confusion matrix contains four important values:

| Actual / Predicted | Positive | Negative |
|---|---:|---:|
| Positive | True Positive (TP) | False Negative (FN) |
| Negative | False Positive (FP) | True Negative (TN) |

### 8.1 True Positive (TP)

True Positive occurs when the actual class is positive and the model also predicts positive.

**Example:** A patient has a disease, and the model correctly predicts that the patient has the disease.

### 8.2 True Negative (TN)

True Negative occurs when the actual class is negative and the model also predicts negative.

**Example:** A patient does not have a disease, and the model correctly predicts that the patient does not have the disease.

### 8.3 False Positive (FP)

False Positive occurs when the actual class is negative, but the model predicts positive.

**Example:** A healthy patient is incorrectly classified as having a disease.

### 8.4 False Negative (FN)

False Negative occurs when the actual class is positive, but the model predicts negative.

**Example:** A patient has a disease, but the model incorrectly predicts that the patient does not have the disease.

## 9. Accuracy

Accuracy measures the percentage of correctly classified predictions out of all predictions.

The formula is:

$$
Accuracy=\frac{TP+TN}{TP+TN+FP+FN}
$$

**Example:**

Suppose:

$$
TP=40,\quad TN=50
$$

$$
FP=5,\quad FN=5
$$

Then:

$$
Accuracy=\frac{40+50}{40+50+5+5}
$$

$$
=\frac{90}{100}
$$

$$
\boxed{Accuracy=90\%}
$$

## 10. Precision

Precision measures how many of the instances predicted as positive are actually positive.

The formula is:

$$
Precision=\frac{TP}{TP+FP}
$$

**Example:**

Suppose:

$$
TP=40,\quad FP=5
$$

Then:

$$
Precision=\frac{40}{40+5}
$$

$$
=\frac{40}{45}
$$

$$
\boxed{Precision=88.89\%}
$$

## 11. Recall (Sensitivity)

Recall measures how many of the actual positive instances are correctly identified by the model.

The formula is:

$$
Recall=\frac{TP}{TP+FN}
$$

**Example:**

Suppose:

$$
TP=40,\quad FN=5
$$

Then:

$$
Recall=\frac{40}{40+5}
$$

$$
=\frac{40}{45}
$$

$$
\boxed{Recall=88.89\%}
$$

## 12. F1-Score

F1-Score is the harmonic mean of Precision and Recall.

It provides a single performance measure by considering both Precision and Recall.

The formula is:

$$
F1=2\times\frac{Precision\times Recall}
{Precision+Recall}
$$

Another formula using confusion matrix values is:

$$
F1=\frac{2TP}{2TP+FP+FN}
$$

**Example:**

Suppose:

$$
Precision=0.8889
$$

$$
Recall=0.8889
$$

Then:

$$
F1=2\times
\frac{0.8889\times0.8889}
{0.8889+0.8889}
$$

$$
\boxed{F1=0.8889=88.89\%}
$$

## 13. Complete Numerical Example of Confusion Matrix

**Problem:**

A classification model produces the following results:

- True Positive (TP) = 80
- True Negative (TN) = 90
- False Positive (FP) = 10
- False Negative (FN) = 20

Calculate Accuracy, Precision, Recall, and F1-Score.

**Solution:**

**Step 1: Calculate Accuracy**

$$
Accuracy=\frac{TP+TN}{TP+TN+FP+FN}
$$

$$
=\frac{80+90}{80+90+10+20}
$$

$$
=\frac{170}{200}
$$

$$
\boxed{Accuracy=85\%}
$$

**Step 2: Calculate Precision**

$$
Precision=\frac{TP}{TP+FP}
$$

$$
=\frac{80}{80+10}
$$

$$
=\frac{80}{90}
$$

$$
\boxed{Precision=88.89\%}
$$

**Step 3: Calculate Recall**

$$
Recall=\frac{TP}{TP+FN}
$$

$$
=\frac{80}{80+20}
$$

$$
=\frac{80}{100}
$$

$$
\boxed{Recall=80\%}
$$

**Step 4: Calculate F1-Score**

$$
F1=\frac{2TP}{2TP+FP+FN}
$$

$$
=\frac{2\times80}{160+10+20}
$$

$$
=\frac{160}{190}
$$

$$
\boxed{F1=84.21\%}
$$

**Final Results:**

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 85% |
| Precision | 88.89% |
| Recall | 80% |
| F1-Score | 84.21% |

## 14. Applications of Naive Bayes and Model Evaluation

1. **Spam Detection:** Identifying spam and non-spam emails.
2. **Sentiment Analysis:** Classifying text as positive, negative, or neutral.
3. **Document Classification:** Categorizing documents based on their content.
4. **Medical Diagnosis:** Predicting diseases based on patient data.
5. **Performance Evaluation:** Measuring how well a classification model performs.
6. **Fraud Detection:** Identifying potentially fraudulent transactions.

## 15. Important Formulas

**Bayes' Theorem:**

$$
P(C|X)=\frac{P(X|C)P(C)}{P(X)}
$$

**Naive Bayes Classification:**

$$
C_{\text{predicted}}=\arg\max_C P(X|C)P(C)
$$

**Accuracy:**

$$
Accuracy=\frac{TP+TN}{TP+TN+FP+FN}
$$

**Precision:**

$$
Precision=\frac{TP}{TP+FP}
$$

**Recall:**

$$
Recall=\frac{TP}{TP+FN}
$$

**F1-Score:**

$$
F1=2\times\frac{Precision\times Recall}
{Precision+Recall}
$$

**Laplace Smoothing:**

$$
P(X_i|C)=
\frac{\text{Count}(X_i,C)+1}
{\text{Total count in C}+V}
$$
