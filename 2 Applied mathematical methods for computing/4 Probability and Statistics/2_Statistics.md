# Statistics - Complete Beginner's Guide

# Table of Contents

1. Statistics vs Probability
2. Gambler's Fallacy
3. Statistical Observations
4. Uniform Distribution
5. Arithmetic Mean
6. Median
7. Mode
8. Sample Size and Confidence
9. Variance
10. Standard Deviation
11. Mean vs Median vs Mode
12. Quick Summary Sheet

---

# Introduction

Probability and statistics are closely related fields of mathematics.

Both deal with:

```text
Uncertainty
Data
Predictions
Patterns
```

However, they answer different questions.

---

# Statistics vs Probability

## Simple Definition

### Probability

Probability studies:

```text
What could happen?
```

It starts with a mathematical model and predicts outcomes.

---

### Statistics

Statistics studies:

```text
What actually happened?
```

It starts with collected data and analyzes it.

---

# Easy Way to Remember

```text
Probability:
Future → Prediction
```

```text
Statistics:
Past/Present → Observation
```

---

# Example 1: Coin Toss

### Probability

Before tossing:

```text
P(Head)=1/2
```

This predicts what could happen.

---

### Statistics

After tossing 100 times:

```text
Heads = 47
Tails = 53
```

This records what actually happened.

---

# Example 2: Weather

### Probability

Weather forecast:

```text
70% chance of rain tomorrow
```

Prediction.

---

### Statistics

Recorded rainfall:

```text
Rain occurred on 21 of 30 days.
```

Observed data.

---

# Example 3: Exams

### Probability

Estimate:

```text
Student has 80% chance of passing.
```

---

### Statistics

Actual results:

```text
72 students passed
28 students failed
```

---

# Visual Comparison

| Probability | Statistics |
|------------|------------|
| What could happen? | What happened? |
| Prediction | Observation |
| Theoretical | Real-world |
| Future-oriented | Data-oriented |

---

# Gambler's Fallacy

## Simple Definition

The Gambler's Fallacy is the false belief that past independent outcomes affect future outcomes.

---

# Key Idea

For independent events:

```text
Past does NOT influence future.
```

---

# Example 1: Coin Toss

Results:

```text
H H H H H
```

Many people think:

```text
Tail is due next.
```

Wrong.

Next toss:

\[
P(T)=\frac12
\]

still.

---

# Example 2: Casino Roulette

Suppose:

```text
Red appears 8 times.
```

People may think:

```text
Black must come next.
```

Wrong.

The wheel has no memory.

---

# Example 3: Rainy Days

Suppose:

```text
Rain for 5 days.
```

People may think:

```text
Tomorrow must be sunny.
```

Not necessarily.

Weather depends on atmospheric conditions, not a balancing rule.

---

# Example 4: Lottery

Numbers:

```text
7 12 24 35 41
```

appeared recently.

Some players avoid them because:

```text
They already appeared.
```

But future draws remain independent.

---

# Statistical Observations

## Simple Definition

A statistical observation is a recorded data point collected from the real world.

Often represented as:

\[
S_1,S_2,S_3,\dots,S_N
\]

---

# Example 1: Exam Scores

Scores:

```text
78
85
92
70
88
```

Observations:

\[
S_1=78
\]

\[
S_2=85
\]

etc.

---

# Example 2: Daily Temperatures

Measurements:

```text
30°C
31°C
29°C
35°C
```

Each measurement is an observation.

---

# Example 3: Dice Rolls

Results:

```text
4
2
6
1
5
```

Each roll is an observation.

---

# Example 4: Website Visits

Daily visitors:

```text
100
120
95
140
```

Each day's count is an observation.

---

# Uniform Distribution

## Simple Definition

A uniform distribution occurs when every outcome has exactly the same probability.

---

# Easy Way to Remember

```text
Uniform = Equal Chance
```

---

# Example 1: Fair Coin

\[
P(H)=P(T)=\frac12
\]

Uniform distribution.

---

# Example 2: Fair Die

\[
P(1)=P(2)=...=P(6)=\frac16
\]

Uniform distribution.

---

# Example 3: Random Card

Each card:

\[
\frac1{52}
\]

Uniform.

---

# Example 4: Lottery Balls

If perfectly designed:

```text
Every number has equal probability.
```

Uniform.

---

# Why Large Samples Matter

Suppose a die is rolled:

```text
6 times
```

Results:

```text
1,1,1,1,2,3
```

Looks unfair.

---

Roll:

```text
1,000,000 times
```

Results become approximately:

```text
1 → 166,667
2 → 166,654
3 → 166,701
...
```

Approaching uniformity.

---

# Arithmetic Mean

## Simple Definition

The arithmetic mean is the average value.

---

# Formula

\[
\text{Mean}
=
\frac1N
\sum_{i=1}^{N}S_i
\]

---

# Easy Way to Remember

```text
Add everything
Divide by count
```

---

# Example 1

Data:

```text
2,4,6
```

Mean:

\[
\frac{2+4+6}{3}
\]

\[
=4
\]

---

# Example 2

Scores:

```text
70,80,90
```

Mean:

\[
80
\]

---

# Example 3

Temperatures:

```text
28,30,32
```

Mean:

\[
30
\]

---

# Example 4

Data:

```text
5,5,5,5
```

Mean:

\[
5
\]

---

# Median

## Simple Definition

The median is the middle value after arranging data in ascending order.

---

# Step 1

Sort data.

---

# Step 2

Find middle value.

---

# Odd Number of Data Points

Use exact middle value.

---

# Example 1

Data:

```text
1,3,5,7,9
```

Middle:

```text
5
```

Median:

\[
5
\]

---

# Example 2

Data:

```text
10,20,30
```

Median:

\[
20
\]

---

# Even Number of Data Points

Take the average of the two middle values.

---

# Example 3

Data:

```text
1,3,5,7
```

Middle values:

```text
3,5
```

Median:

\[
\frac{3+5}{2}
\]

\[
=4
\]

---

# Example 4

Data:

```text
10,20,30,40
```

Median:

\[
25
\]

---

# Why Median Is Useful

Consider:

```text
10
12
13
15
1000
```

Mean:

\[
210
\]

Median:

\[
13
\]

Median better represents the typical value.

---

# Mode

## Simple Definition

The mode is the most frequently occurring value.

---

# Easy Way to Remember

```text
Most Frequent
```

---

# Example 1

Data:

```text
2,2,3,4,5
```

Mode:

```text
2
```

---

# Example 2

Data:

```text
1,1,1,1,7
```

Mode:

```text
1
```

---

# Example 3

Data:

```text
5,6,6,7,8
```

Mode:

```text
6
```

---

# Example 4

Data:

```text
2,2,3,3,4
```

Modes:

```text
2 and 3
```

This is called:

```text
Bimodal
```

---

# Sample Size and Confidence

## Simple Definition

Larger samples generally produce more reliable conclusions.

---

# Easy Way to Remember

```text
More Data
=
More Confidence
```

---

# Example 1: Coin Toss

Toss:

```text
10 times
```

Possible result:

```text
7 Heads
3 Tails
```

Not very reliable.

---

Toss:

```text
100,000 times
```

Possible result:

```text
50,012 Heads
49,988 Tails
```

Much more reliable.

---

# Example 2: Election Poll

Survey:

```text
5 people
```

Poor confidence.

---

Survey:

```text
5000 people
```

Much better confidence.

---

# Example 3: Product Reviews

Review count:

```text
3 reviews
```

Not enough evidence.

---

Review count:

```text
50,000 reviews
```

Far more trustworthy.

---

# Variance (S²)

## Simple Definition

Variance measures how spread out the data is around the mean.

---

# Easy Way to Remember

```text
Variance = Average Squared Distance from Mean
```

---

# Formula

\[
\text{Variance}
=
\frac{\sum(S_i-m)^2}{N}
\]

where:

\[
m
=
\text{mean}
\]

---

# Example 1

Data:

```text
5,5,5
```

Mean:

\[
5
\]

Differences:

```text
0,0,0
```

Squared:

```text
0,0,0
```

Variance:

\[
0
\]

Perfectly consistent.

---

# Example 2

Data:

```text
4,5,6
```

Mean:

\[
5
\]

Differences:

```text
-1,0,1
```

Squares:

```text
1,0,1
```

Variance:

\[
\frac{2}{3}
\]

---

# Example 3

Data:

```text
0,10
```

Mean:

\[
5
\]

Squares:

```text
25,25
```

Variance:

\[
25
\]

Large spread.

---

# Example 4

Data:

```text
50,50,50,50
```

Variance:

\[
0
\]

No spread.

---

# Standard Deviation (S)

## Simple Definition

Standard deviation measures spread using the same units as the original data.

---

# Formula

\[
S
=
\sqrt{\text{Variance}}
\]

---

# Why Use It?

Variance uses squared units.

Standard deviation converts back to original units.

---

# Example 1

Variance:

\[
9
\]

Standard deviation:

\[
3
\]

---

# Example 2

Variance:

\[
16
\]

Standard deviation:

\[
4
\]

---

# Example 3

Variance:

\[
25
\]

Standard deviation:

\[
5
\]

---

# Example 4

Variance:

\[
0
\]

Standard deviation:

\[
0
\]

---

# Mean vs Median vs Mode

| Measure | Meaning |
|----------|----------|
| Mean | Average |
| Median | Middle value |
| Mode | Most frequent value |

---

# Example

Data:

```text
1,2,2,3,10
```

Mean:

\[
\frac{18}{5}
=
3.6
\]

Median:

\[
2
\]

Mode:

\[
2
\]

---

# Quick Summary Sheet

## Probability

Studies:

```text
What could happen?
```

---

## Statistics

Studies:

```text
What actually happened?
```

---

## Gambler's Fallacy

False belief that past independent outcomes affect future outcomes.

---

## Statistical Observation

Single recorded data value.

\[
S_i
\]

---

## Uniform Distribution

All outcomes equally likely.

---

## Arithmetic Mean

\[
\frac1N\sum S_i
\]

Average value.

---

## Median

Middle value after sorting.

---

## Mode

Most common value.

---

## Sample Size

Larger samples produce higher confidence.

---

## Variance

\[
\frac{\sum(S_i-m)^2}{N}
\]

Measures spread.

---

## Standard Deviation

\[
\sqrt{\text{Variance}}
\]

Measures spread in original units.

---

# Golden Rules

### Probability

```text
Predict
```

---

### Statistics

```text
Observe
```

---

### Mean

```text
Average
```

---

### Median

```text
Middle
```

---

### Mode

```text
Most Frequent
```

---

### Variance

```text
Spread Squared
```

---

### Standard Deviation

```text
Spread
```

---

### Confidence

```text
More Data = Better Confidence
```

These ideas form the foundation of descriptive statistics, data analysis, machine learning, data science, and modern analytics.