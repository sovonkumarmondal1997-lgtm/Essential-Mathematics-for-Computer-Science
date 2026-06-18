# Advanced Counting Techniques

# Table of Contents

1. Complement Counting Principle
2. Sum Rule of Counting with Independent Disjoint Sets
3. Permutations with Repetition (Alphanumeric Combinations)
4. Inclusion-Exclusion Principle (Subtraction Rule)
5. Divisibility Counting via Multiples
6. Floor Function
7. Least Common Multiple (LCM) in Counting Intersections
8. Quick Summary Sheet

---

# Complement Counting Principle

## Simple Definition

Sometimes counting the outcomes we want is difficult.

Instead of counting the desired outcomes directly, we:

1. Count all possible outcomes.
2. Count the unwanted outcomes.
3. Subtract.

Formula:

\[
\text{Desired Outcomes}
=
\text{Total Outcomes}
-
\text{Unwanted Outcomes}
\]

---

## Why Use It?

Sometimes:

```text
Direct counting = Difficult
```

but

```text
Counting the opposite = Easy
```

In such cases, complement counting saves time.

---

# Example 1: Password with At Least One Uppercase Letter

Suppose:

- Password length = 4
- Characters can be:
  - 26 uppercase letters
  - 26 lowercase letters

Total characters:

\[
52
\]

---

## Step 1: Count Total Passwords

Each position has 52 choices.

\[
52^4
\]

\[
7,311,616
\]

---

## Step 2: Count Passwords With No Uppercase Letters

Only lowercase allowed.

\[
26^4
\]

\[
456,976
\]

---

## Step 3: Subtract

\[
52^4 - 26^4
\]

\[
7,311,616 - 456,976
\]

\[
6,854,640
\]

### Answer

```text
6,854,640 passwords contain at least one uppercase letter.
```

---

# Example 2: At Least One Head

Flip a coin 5 times.

How many outcomes contain at least one head?

---

## Total Outcomes

\[
2^5 = 32
\]

---

## Unwanted Outcomes

No heads at all:

```text
TTTTT
```

Only 1 outcome.

---

## Subtract

\[
32 - 1 = 31
\]

### Answer

```text
31 outcomes contain at least one head.
```

---

# Example 3: At Least One Digit 5

Create a 3-digit code.

Digits:

```text
0-9
```

How many codes contain at least one digit 5?

---

## Total

\[
10^3=1000
\]

---

## No Digit 5

Each position has:

\[
9
\]

choices.

\[
9^3=729
\]

---

## Desired

\[
1000-729=271
\]

### Answer

```text
271 codes contain at least one digit 5.
```

---

# Sum Rule of Counting with Independent Disjoint Sets

## Simple Definition

When a problem can be divided into separate cases that cannot happen simultaneously, count each case separately and add them.

Formula:

\[
n(A)+n(B)+n(C)+...
\]

---

## Key Idea

The cases must be:

```text
Mutually Exclusive
```

Meaning:

```text
No overlap
```

---

# Example 1: Password Length

Suppose passwords may have:

```text
Length 5
OR
Length 6
OR
Length 7
```

Each position:

```text
26 letters
```

---

## Length 5

\[
26^5
\]

\[
11,881,376
\]

---

## Length 6

\[
26^6
\]

\[
308,915,776
\]

---

## Length 7

\[
26^7
\]

\[
8,031,810,176
\]

---

## Total

\[
26^5+26^6+26^7
\]

\[
8,352,607,328
\]

### Answer

```text
8,352,607,328 passwords
```

---

# Example 2: Choosing a Vehicle

You can choose:

```text
3 bikes
OR
5 cars
OR
2 trucks
```

Total:

\[
3+5+2=10
\]

### Answer

```text
10 choices
```

---

# Example 3: Student Selection

Choose:

```text
Freshman
OR
Sophomore
OR
Junior
```

Suppose:

```text
50 freshmen
40 sophomores
30 juniors
```

Total:

\[
50+40+30
\]

\[
120
\]

### Answer

```text
120 students
```

---

# Permutations with Repetition (Alphanumeric Combinations)

## Simple Definition

Suppose:

```text
Letters A-Z
Digits 0-9
```

Total symbols:

\[
26+10=36
\]

If repetition is allowed, every position has 36 choices.

Formula:

\[
36^n
\]

where:

\[
n = \text{number of positions}
\]

---

# Example 1: 4-Character Code

Each position:

\[
36
\]

choices.

\[
36^4
\]

\[
1,679,616
\]

### Answer

```text
1,679,616 codes
```

---

# Example 2: 6-Character Password

\[
36^6
\]

\[
2,176,782,336
\]

### Answer

```text
2.17 billion passwords
```

---

# Example 3: Vehicle Tag

Format:

```text
XXXXXX
```

where each position is:

```text
Letter or Digit
```

\[
36^6
\]

\[
2,176,782,336
\]

### Answer

```text
2.17 billion tags
```

---

# Inclusion-Exclusion Principle
## (Subtraction Rule)

## Simple Definition

When counting:

```text
A OR B
```

some elements may belong to both groups.

If we simply add:

\[
n(A)+n(B)
\]

we count the overlap twice.

Therefore:

\[
n(A\cup B)
=
n(A)+n(B)-n(A\cap B)
\]

---

# Visual Idea

```text
Set A       Set B

  *****---*****
      overlap
```

Overlap gets counted twice.

Subtract once.

---

# Example 1: Students

Suppose:

```text
20 play Cricket
15 play Football
5 play Both
```

Total students playing at least one sport:

\[
20+15-5
\]

\[
30
\]

### Answer

```text
30 students
```

---

# Example 2: Divisible by 2 or 3

Numbers:

```text
1 to 20
```

---

## Multiples of 2

\[
10
\]

---

## Multiples of 3

\[
6
\]

---

## Multiples of Both

Multiples of:

\[
6
\]

There are:

\[
3
\]

---

## Inclusion-Exclusion

\[
10+6-3
\]

\[
13
\]

### Answer

```text
13 numbers are divisible by 2 or 3.
```

---

# Example 3: Club Membership

Suppose:

```text
40 in Music Club
25 in Drama Club
10 in Both
```

Total:

\[
40+25-10
\]

\[
55
\]

### Answer

```text
55 students
```

---

# Divisibility Counting via Multiples

## Simple Definition

We often need to count how many numbers in a range are divisible by a number d.

Examples:

```text
How many numbers from 1 to 100 are divisible by 5?
```

---

## Basic Formula

\[
\left\lfloor\frac{N}{d}\right\rfloor
\]

where:

- N = upper limit
- d = divisor

---

# Example 1: Multiples of 5

Range:

```text
1 to 100
```

\[
\left\lfloor\frac{100}{5}\right\rfloor
\]

\[
20
\]

### Answer

```text
20 numbers
```

---

# Example 2: Multiples of 7

Range:

```text
1 to 50
```

\[
\left\lfloor\frac{50}{7}\right\rfloor
\]

\[
7
\]

Multiples:

```text
7
14
21
28
35
42
49
```

### Answer

```text
7 numbers
```

---

# Example 3: Multiples of 3

Range:

```text
1 to 1000
```

\[
\left\lfloor\frac{1000}{3}\right\rfloor
\]

\[
333
\]

### Answer

```text
333 numbers
```

---

# Floor Function

## Symbol

\[
\lfloor x \rfloor
\]

Read as:

```text
Floor of x
```

---

## Simple Definition

The floor function returns:

```text
Greatest integer less than or equal to x
```

Simply:

```text
Remove the decimal part
```

---

# Examples

## Example 1

\[
\lfloor 3.9 \rfloor = 3
\]

---

## Example 2

\[
\lfloor 8.2 \rfloor = 8
\]

---

## Example 3

\[
\lfloor 5 \rfloor = 5
\]

---

## Example 4

\[
\lfloor -2.3 \rfloor = -3
\]

Notice:

```text
Not -2
```

because floor moves downward.

---

# Why Floor Is Used in Counting

Suppose:

\[
100/7
=
14.2857
\]

There cannot be:

```text
14.2857 multiples
```

Only whole numbers count.

Therefore:

\[
\lfloor 100/7\rfloor
=
14
\]

---

# Least Common Multiple (LCM) in Counting Intersections

## Simple Definition

When counting numbers divisible by:

```text
A and B
```

we find the LCM.

Why?

Because numbers divisible by both must be multiples of the LCM.

---

# Example 1: Divisible by 2 and 3

Multiples:

```text
2:
2,4,6,8,10,...

3:
3,6,9,12,...
```

Common multiples:

```text
6,12,18,...
```

LCM:

\[
6
\]

---

# Example 2: Divisible by 4 and 6

Multiples:

```text
4:
4,8,12,16,20,24...

6:
6,12,18,24...
```

Common:

```text
12,24,...
```

LCM:

\[
12
\]

---

# Example 3: Numbers from 1 to 100 Divisible by Both 2 and 3

LCM:

\[
6
\]

Count:

\[
\left\lfloor \frac{100}{6}\right\rfloor
\]

\[
16
\]

### Answer

```text
16 numbers
```

---

# Example 4: Numbers from 1 to 200 Divisible by Both 4 and 6

LCM:

\[
12
\]

Count:

\[
\left\lfloor \frac{200}{12}\right\rfloor
\]

\[
16
\]

### Answer

```text
16 numbers
```

---

# Quick Summary Sheet

## Complement Counting Principle

\[
\text{Desired}
=
\text{Total}
-
\text{Unwanted}
\]

Used for:

```text
At least one...
```

problems.

---

## Sum Rule

\[
n(A)+n(B)+n(C)
\]

Used when cases are:

```text
Mutually Exclusive
```

---

## Alphanumeric Permutations

\[
36^n
\]

because:

```text
26 letters + 10 digits = 36 symbols
```

---

## Inclusion-Exclusion

\[
n(A\cup B)
=
n(A)+n(B)-n(A\cap B)
\]

Remember:

```text
Subtract overlap once
```

---

## Divisibility Counting

\[
\left\lfloor \frac{N}{d} \right\rfloor
\]

Counts multiples of d up to N.

---

## Floor Function

\[
\lfloor x \rfloor
\]

Largest integer less than or equal to x.

---

## LCM in Counting

To count numbers divisible by both A and B:

1. Find LCM(A,B)
2. Count multiples of the LCM

\[
\left\lfloor \frac{N}{LCM(A,B)} \right\rfloor
\]

---

# Golden Rules

### AND → Multiply

\[
m \times n
\]

### OR → Add

\[
m+n
\]

### At Least One → Use Complement

\[
\text{Total} - \text{None}
\]

### A OR B With Overlap

Use Inclusion-Exclusion:

\[
A+B-\text{Overlap}
\]

### Divisible By Both

Use:

\[
LCM
\]

then count multiples.