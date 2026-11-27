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

**END OF LECTURE 11**
