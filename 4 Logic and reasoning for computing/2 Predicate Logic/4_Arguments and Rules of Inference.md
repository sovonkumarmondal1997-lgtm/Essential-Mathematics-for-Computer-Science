# Arguments and Rules of Inference - Beginner Friendly Notes

# 1. Argument

An **argument** is a group of statements where some statements (called
**premises**) are used to support another statement called the
**conclusion**.

Structure:

Premise 1

Premise 2

...

Conclusion

Example:

Premise 1: If it rains, the road gets wet.

Premise 2: It is raining.

Conclusion: Therefore, the road is wet.

------------------------------------------------------------------------

# 2. Valid Argument

A valid argument has a correct logical structure.

If all premises are true, the conclusion **must** be true.

Example:

If I study, I pass.

I study.

Therefore, I pass.

This is valid.

Another Example:

All humans are mortal.

Socrates is a human.

Therefore, Socrates is mortal.

------------------------------------------------------------------------

# 3. Fallacy (Formal Fallacy)

A fallacy is an incorrect pattern of reasoning.

Even if the conclusion happens to be true, the logic is invalid.

Example:

If it rains, roads become wet.

Roads are wet.

Therefore, it rained.

Wrong.

Someone may have washed the road.

------------------------------------------------------------------------

# 4. Modus Ponens

Rule:

(P → Q) ∧ P ⇒ Q

Meaning:

If the condition is true and the condition actually happened, then the
result must happen.

Example:

If I exercise, I become healthy.

I exercise.

Therefore,

I become healthy.

Example:

If a number is divisible by 4, it is even.

16 is divisible by 4.

Therefore,

16 is even.

------------------------------------------------------------------------

# 5. Modus Tollens

Rule:

(P → Q) ∧ ¬Q ⇒ ¬P

Meaning:

If the result did not happen, then the condition never happened.

Example:

If I study, I pass.

I did not pass.

Therefore,

I did not study.

Example:

If a file exists, it can be opened.

The file cannot be opened.

Therefore,

The file does not exist.

------------------------------------------------------------------------

# 6. Conjunction

Rule:

P

Q

Therefore,

P ∧ Q

Meaning:

If two facts are true individually, we may join them using AND.

Example:

Python is popular.

SQL is popular.

Therefore,

Python AND SQL are popular.

------------------------------------------------------------------------

# 7. Simplification

Rule:

P ∧ Q ⇒ P

or

P ∧ Q ⇒ Q

Meaning:

If both are true together, either one is individually true.

Example:

Alice studies AND Alice exercises.

Therefore,

Alice studies.

Also,

Alice exercises.

------------------------------------------------------------------------

# 8. Addition

Rule:

P ⇒ P ∨ Q

Meaning:

If one statement is true, then "P OR anything" is also true.

Example:

Today is Sunday.

Therefore,

Today is Sunday OR it is snowing.

The OR statement remains true because the first part is already true.

------------------------------------------------------------------------

# 9. Hypothetical Syllogism

Rule:

(P → Q) ∧ (Q → R)

⇒

P → R

Meaning:

Chain implications together.

Example:

If I study,

I pass.

If I pass,

I get a job.

Therefore,

If I study,

I get a job.

Example:

If water freezes,

it becomes ice.

If it becomes ice,

it becomes solid.

Therefore,

If water freezes,

it becomes solid.

------------------------------------------------------------------------

# 10. Disjunctive Syllogism

Rule:

(P ∨ Q) ∧ ¬P ⇒ Q

Meaning:

If one choice is impossible, the other must be true.

Example:

Today is Saturday OR Sunday.

Today is not Saturday.

Therefore,

Today is Sunday.

Example:

The switch is ON or OFF.

It is not ON.

Therefore,

It is OFF.

------------------------------------------------------------------------

# 11. Resolution

Rule:

(P ∨ Q)

(¬P ∨ R)

Therefore,

Q ∨ R

Meaning:

Cancel opposite terms and combine what remains.

Example:

Either Alice studies OR Bob studies.

Either Alice does not study OR Charlie studies.

Therefore,

Bob studies OR Charlie studies.

Example:

Server A works OR Server B works.

Server A fails OR Backup starts.

Therefore,

Server B works OR Backup starts.

------------------------------------------------------------------------

# 12. Argument Construction Proof

Steps:

1.  Translate English into symbols.
2.  Identify premises.
3.  Apply inference rules.
4.  Reach the conclusion.

Example

Premise:

If it rains, roads become wet.

Premise:

If roads become wet, traffic slows.

Premise:

It rains.

Step 1

Modus Ponens

Roads become wet.

Step 2

Modus Ponens

Traffic slows.

Conclusion proved.

------------------------------------------------------------------------

# 13. Affirming the Consequent (Fallacy)

Incorrect Rule:

(P → Q)

Q

Therefore,

P

This is INVALID.

Example:

If I study,

I pass.

I passed.

Therefore,

I studied.

Wrong.

Maybe I passed because of prior knowledge.

Example:

If it rains,

roads become wet.

Roads are wet.

Therefore,

It rained.

Wrong.

Someone may have cleaned the road.

------------------------------------------------------------------------

# Comparison Table

  Rule                       Formula            Meaning
  -------------------------- ------------------ ---------------------
  Modus Ponens               (P→Q)∧P⇒Q          Confirm condition
  Modus Tollens              (P→Q)∧¬Q⇒¬P        Reject condition
  Conjunction                P,Q⇒P∧Q            Join facts
  Simplification             P∧Q⇒P              Extract one fact
  Addition                   P⇒P∨Q              Add OR
  Hypothetical Syllogism     (P→Q),(Q→R)⇒P→R    Chain implications
  Disjunctive Syllogism      (P∨Q),¬P⇒Q         Remove false choice
  Resolution                 (P∨Q),(¬P∨R)⇒Q∨R   Combine clauses
  Affirming the Consequent   (P→Q),Q⇒P          Invalid

------------------------------------------------------------------------

# Memory Tricks

-   Argument = Premises + Conclusion.
-   Valid argument = Impossible for true premises to give a false
    conclusion.
-   Modus Ponens = Condition happened.
-   Modus Tollens = Result failed.
-   Conjunction = Join facts.
-   Simplification = Split AND.
-   Addition = Add OR.
-   Hypothetical Syllogism = Chain implications.
-   Disjunctive Syllogism = Remove impossible choice.
-   Resolution = Cancel opposite literals.
-   Affirming the Consequent = Common logical mistake.

These inference rules are widely used in mathematics, theorem proving,
programming, SQL query optimization, artificial intelligence, expert
systems, and formal verification.
