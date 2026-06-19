# Proof of the Power Rule Using the Binomial Theorem

---

# Introduction

So far, we have proven:

\[
\frac{d}{dx}(x^2)=2x
\]

and

\[
\frac{d}{dx}(x^3)=3x^2
\]

by using first principles.

A natural question now arises:

> Can we prove the derivative of ANY power of \(x\)?

Examples:

\[
x^4,\quad x^5,\quad x^{10},\quad x^{100}
\]

Instead of proving each one individually, mathematicians use the **Binomial Theorem** to prove a single universal rule:

\[
\boxed{
\frac{d}{dx}(x^n)=nx^{n-1}
}
\]

This is called the **Power Rule**.

---

# 1. Purpose of the Binomial Theorem in Calculus

---

## Why Do We Need the Binomial Theorem?

For:

\[
x^2
\]

we expanded:

\[
(x+\Delta x)^2
\]

directly.

For:

\[
x^3
\]

we expanded:

\[
(x+\Delta x)^3
\]

directly.

---

But what about:

\[
x^{50}
\]

or

\[
x^{1000}
\]

Expanding manually would be impossible.

---

The Binomial Theorem provides a universal expansion for:

\[
(x+\Delta x)^n
\]

regardless of the value of \(n\).

---

# Example

Instead of writing:

\[
(x+\Delta x)^4
\]

by hand,

the theorem instantly gives:

\[
x^4
+
4x^3\Delta x
+
6x^2(\Delta x)^2
+
4x(\Delta x)^3
+
(\Delta x)^4
\]

---

# Real-Life Analogy

Imagine multiplying large numbers.

Instead of adding repeatedly:

\[
5+5+5+5+5
\]

you use:

\[
5\times5
\]

The Binomial Theorem is a shortcut for enormous algebraic expansions.

---

# Easy Memory Rule

**The Binomial Theorem is the bridge between simple examples and the general derivative of \(x^n\).**

---

# 2. Setting Up First Principles for \(x^n\)

---

## Start with the Function

\[
f(x)=x^n
\]

---

# Apply the First-Principles Formula

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
f(x+\Delta x)-f(x)
}
{\Delta x}
\]

---

Substitute:

\[
f(x)=x^n
\]

---

Result:

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
(x+\Delta x)^n
-
x^n
}
{\Delta x}
\]

---

This is where the proof begins.

---

# Why Can't We Continue Immediately?

Because:

\[
(x+\Delta x)^n
\]

is too complicated.

We must expand it.

---

This is where the Binomial Theorem enters.

---

# Easy Memory Rule

**First Principles gives the framework; the Binomial Theorem does the heavy algebra.**

---

# 3. Canceling the Leading Terms

---

# Expand Using the Binomial Theorem

The beginning of the expansion is:

\[
(x+\Delta x)^n
=
x^n
+
nx^{n-1}\Delta x
+
\cdots
\]

---

Substitute into the derivative formula:

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
x^n
+
nx^{n-1}\Delta x
+
\cdots
-
x^n
}
{\Delta x}
\]

---

# Notice Something Important

We have:

\[
+x^n
\]

and

\[
-x^n
\]

---

They cancel perfectly.

---

Result:

\[
=
\lim_{\Delta x\to0}
\frac{
nx^{n-1}\Delta x
+
\cdots
}
{\Delta x}
\]

---

# Example with \(n=4\)

Expansion:

\[
(x+h)^4
=
x^4
+
4x^3h
+
6x^2h^2
+
4xh^3
+
h^4
\]

---

Derivative expression:

\[
\frac{
x^4
+
4x^3h
+
6x^2h^2
+
4xh^3
+
h^4
-
x^4
}
{h}
\]

---

The \(x^4\) terms disappear.

---

# Why Is This Important?

Without this cancellation, the proof would never simplify.

---

# Real-Life Analogy

Imagine carrying a heavy backpack.

Before running, you remove the backpack.

The largest weight disappears.

The proof becomes much easier.

---

# Easy Memory Rule

**The first \(x^n\) always cancels the last \(x^n\).**

---

# 4. The Dominance of the Second Term

---

After cancellation:

\[
nx^{n-1}\Delta x
+
\text{other terms}
\]

becomes the new leading term.

---

# Why Is This Special?

It contains:

\[
\Delta x
\]

to the first power only.

---

All later terms contain:

\[
(\Delta x)^2
\]

or

\[
(\Delta x)^3
\]

or higher powers.

---

# Example

For:

\[
(x+h)^5
\]

the expansion begins:

\[
x^5
+
5x^4h
+
10x^3h^2
+
10x^2h^3
+\cdots
\]

---

After cancellation:

\[
5x^4h
+
10x^3h^2
+\cdots
\]

---

The first surviving term:

\[
5x^4h
\]

is the most important term.

---

# Why Do Mathematicians Care About It?

Because after division by \(h\),

it becomes:

\[
5x^4
\]

with no \(h\) remaining.

---

# Real-Life Analogy

Imagine a competition where many contestants enter.

One contestant has a huge advantage.

That contestant survives until the end.

The second term is that contestant.

---

# Easy Memory Rule

**The second term contains exactly one \(\Delta x\), making it the future derivative.**

---

# 5. Eliminating Higher-Order \(\Delta x\) Terms

---

After cancellation we divide by:

\[
\Delta x
\]

---

Expression:

\[
\frac{
nx^{n-1}\Delta x
+
A(\Delta x)^2
+
B(\Delta x)^3
+\cdots
}
{\Delta x}
\]

---

Divide every term.

---

First term:

\[
\frac{
nx^{n-1}\Delta x
}
{\Delta x}
=
nx^{n-1}
\]

---

Second term:

\[
\frac{
A(\Delta x)^2
}
{\Delta x}
=
A\Delta x
\]

---

Third term:

\[
\frac{
B(\Delta x)^3
}
{\Delta x}
=
B(\Delta x)^2
\]

---

Notice what happened.

---

The first term lost all \(\Delta x\).

But every later term still contains at least one \(\Delta x\).

---

# Example

Suppose:

\[
\frac{
3x^2h
+
3xh^2
+
h^3
}
{h}
\]

---

Divide:

\[
=
3x^2
+
3xh
+
h^2
\]

---

The first term survives completely.

The others still contain \(h\).

---

# Why Is This Important?

Because the limit is about to send:

\[
h
\rightarrow0
\]

---

# Real-Life Analogy

Imagine filtering sand through a sieve.

Large particles remain.

Tiny particles fall through.

The derivative survives while higher-order terms disappear.

---

# Easy Memory Rule

**After dividing by \(\Delta x\), only the first surviving term loses all \(\Delta x\).**

---

# 6. Evaluating the Limit to Prove the Power Rule

---

After simplification:

\[
f'(x)
=
\lim_{\Delta x\to0}
\left[
nx^{n-1}
+
A\Delta x
+
B(\Delta x)^2
+\cdots
\right]
\]

---

Now apply:

\[
\Delta x\to0
\]

---

# What Happens?

---

## First Term

\[
nx^{n-1}
\]

contains no \(\Delta x\).

Nothing changes.

---

## Second Term

\[
A\Delta x
\]

becomes:

\[
0
\]

---

## Third Term

\[
B(\Delta x)^2
\]

becomes:

\[
0
\]

---

All remaining terms vanish.

---

# Final Result

\[
f'(x)
=
nx^{n-1}
\]

---

# The Power Rule

\[
\boxed{
\frac{d}{dx}(x^n)
=
nx^{n-1}
}
\]

---

# Example 1

\[
\frac{d}{dx}(x^2)
\]

---

Apply the rule:

\[
2x^{2-1}
\]

---

Answer:

\[
2x
\]

---

# Example 2

\[
\frac{d}{dx}(x^3)
\]

---

Answer:

\[
3x^2
\]

---

# Example 3

\[
\frac{d}{dx}(x^5)
\]

---

Answer:

\[
5x^4
\]

---

# Example 4

\[
\frac{d}{dx}(x^{10})
\]

---

Answer:

\[
10x^9
\]

---

# Example 5

\[
\frac{d}{dx}(x^{100})
\]

---

Answer:

\[
100x^{99}
\]

---

# Why Is This One of the Greatest Results in Calculus?

Before this proof:

Every power required a separate derivation.

After this proof:

One simple rule differentiates every polynomial power.

---

# Real-Life Example

Suppose:

\[
s(t)=t^5
\]

represents distance.

---

Velocity:

\[
v(t)=5t^4
\]

---

Suppose:

\[
P(x)=x^{20}
\]

represents profit.

---

Growth rate:

\[
P'(x)=20x^{19}
\]

---

The same rule works everywhere.

---

# Complete Summary

---

## Step 1

Start with:

\[
f(x)=x^n
\]

and substitute into first principles.

---

## Step 2

Expand:

\[
(x+\Delta x)^n
\]

using the Binomial Theorem.

---

## Step 3

The leading:

\[
x^n
\]

cancels.

---

## Step 4

The second term:

\[
nx^{n-1}\Delta x
\]

becomes dominant.

---

## Step 5

Divide by:

\[
\Delta x
\]

The first surviving term loses all \(\Delta x\).

---

## Step 6

Take the limit:

\[
\Delta x\to0
\]

All remaining terms vanish.

---

## Final Result

\[
\boxed{
\frac{d}{dx}(x^n)
=
nx^{n-1}
}
\]

---

### One-Sentence Memory Rule

**The Binomial Theorem reveals that after expanding \((x+\Delta x)^n\), canceling \(x^n\), dividing by \(\Delta x\), and taking the limit, every term disappears except \(nx^{n-1}\), proving the Power Rule \(\frac{d}{dx}(x^n)=nx^{n-1}\).**