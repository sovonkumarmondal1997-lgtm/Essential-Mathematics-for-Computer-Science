# Stable Matching and Gale-Shapley Algorithm

These notes explain the Stable Matching Problem and the Gale-Shapley
algorithm using simple language, analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Stable Matching Problem

A **Stable Matching Problem** asks how to pair two equally sized groups
(for example, hospitals and students) so everyone is matched and no pair
wishes to leave their assigned partners.

## Example

Hospitals: - H1 - H2

Students: - S1 - S2

Preferences

H1: S1 \> S2

H2: S2 \> S1

S1: H1 \> H2

S2: H2 \> H1

Matching:

H1--S1

H2--S2

Everyone gets their favorite choice.

------------------------------------------------------------------------

# 2. Unstable Pair

An **unstable pair** is a hospital and student who are not matched
together but both prefer each other over their current partners.

Example

Current matching:

H1--S2

H2--S1

If H1 prefers S1 and S1 prefers H1, they would rather be together.

This makes the matching unstable.

Analogy: Two dance partners secretly wishing to swap partners.

------------------------------------------------------------------------

# 3. Stable Matching

A **stable matching** has **no unstable pairs**.

Nobody has an incentive to leave their assigned partner.

Example:

H1--S1

H2--S2

If no hospital-student pair wants to switch, the matching is stable.

------------------------------------------------------------------------

# 4. Perfect Matching

A **perfect matching** means every participant is matched exactly once.

If there are n hospitals and n students:

\|Matching\| = n

Example:

3 hospitals

3 students

Every hospital gets one student and every student gets one hospital.

------------------------------------------------------------------------

# 5. Gale-Shapley Algorithm

The **Gale-Shapley Algorithm** (Deferred Acceptance) works like this:

1.  Every unmatched hospital proposes to its highest-ranked student not
    yet rejected.
2.  Each student temporarily keeps the best offer received so far.
3.  Worse offers are rejected.
4.  Rejected hospitals propose again.
5.  Continue until everyone is matched.

## Example

Round 1

H1 → S1

H2 → S1

S1 prefers H2.

Keeps H2.

Rejects H1.

Round 2

H1 → S2

S2 accepts.

Final:

H1--S2

H2--S1

------------------------------------------------------------------------

# 6. Gale-Shapley Pseudocode Strategy

Simple pseudocode

START

Initialize all hospitals unmatched.

WHILE an unmatched hospital still has someone to propose to

    Propose to the next student.

    IF student is free

        Accept proposal.

    ELSE

        Student compares current match with new proposal.

        Keep the preferred hospital.

        Reject the other.

END WHILE

STOP

------------------------------------------------------------------------

# 7. Termination Proof (n² Upper Bound)

Each hospital can propose to each student **at most once**.

With n hospitals and n students:

Maximum proposals = n × n = n².

Therefore, the algorithm must stop.

Example:

3 hospitals

3 students

Maximum proposals = 9.

Even in the worst case, no more than 9 proposals occur.

------------------------------------------------------------------------

# 8. Perfect Matching Proof (By Contradiction)

Idea:

Assume the algorithm finishes with one hospital unmatched.

That hospital must have proposed to every student.

Every student must already be matched.

Therefore there cannot actually be an unmatched hospital.

This contradiction proves everyone gets matched.

------------------------------------------------------------------------

# 9. Stability Proof (By Contradiction)

Assume an unstable pair exists.

Hospital H prefers Student S.

Student S also prefers Hospital H.

If this were true:

-   H must have proposed to S before proposing to anyone lower.
-   S would either have accepted H or later rejected H for an even
    better hospital.

Therefore S cannot prefer H over the final partner.

Contradiction.

Hence the matching is stable.

------------------------------------------------------------------------

# 10. Stable Matching Variations

Real-world matching problems are often more complex.

Examples:

-   Unequal numbers of hospitals and students.
-   Hospitals with multiple vacancies.
-   Couples wanting nearby hospitals.
-   Participants listing only acceptable partners.

Example:

Hospital H1 has two available positions.

It can accept two students instead of one.

------------------------------------------------------------------------

# Complete Worked Example

Hospitals:

H1: S1 \> S2

H2: S1 \> S2

Students:

S1: H2 \> H1

S2: H1 \> H2

Round 1

H1 → S1

H2 → S1

S1 keeps H2.

Rejects H1.

Round 2

H1 → S2

S2 accepts.

Final Matching

H1--S2

H2--S1

No unstable pair exists.

------------------------------------------------------------------------

# Time Complexity

Worst-case proposals:

O(n²)

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                             Simple Meaning
  ----------------------------------- -----------------------------------
  Stable Matching Problem             Pair two groups using preferences

  Unstable Pair                       Two unmatched people prefer each
                                      other

  Stable Matching                     No unstable pairs exist

  Perfect Matching                    Everyone is matched exactly once

  Gale-Shapley Algorithm              Repeated proposals until stable
                                      matching

  Pseudocode Strategy                 Propose, accept temporarily, reject
                                      weaker offers

  Termination Proof                   At most n² proposals

  Perfect Matching Proof              Everyone must eventually be matched

  Stability Proof                     No blocking pair can remain

  Stable Matching Variations          Extensions with capacities, unequal
                                      sizes, couples, etc.
  -----------------------------------------------------------------------
